# Oscilações Acústicas de Bárions: Códigos dos Resultados

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22217922.svg)](https://doi.org/10.5281/zenodo.22217922)

Este repositório contém os notebooks Python que geram os resultados
numéricos apresentados no Trabalho de Conclusão de Curso **"Ondas
Sonoras Congeladas no Tempo: A RCF Como Régua Cósmica"**, de
Johnatans Neves Souza (2026), sobre a física das Oscilações Acústicas
de Bárions (OABs) e o uso da radiação cósmica de fundo (RCF) como
régua padrão cosmológica.

Cada notebook implementa e verifica numericamente um resultado
específico do Capítulo de Resultados do TCC, com verificação
sistemática contra valores de referência do Planck 2018 e fórmulas de
ajuste de Eisenstein & Hu (1998).

## Estrutura do repositório

| Notebook | Resultado no TCC | Descrição |
|---|---|---|
| `Resultado 01-SHOA.ipynb` | Resultado 1 | Solução Homogênea do Oscilador Acústico, sem forçante nem amortecimento, para três números de onda representativos. |
| `Resultado 02-OFAP.ipynb` | Resultado 2 | Oscilador Forçado e Assimetria dos Picos: potencial gravitacional constante e assimetria entre picos pares e ímpares em função da razão bárion-fóton $R$. |
| `Resultado 03-ASAOR.ipynb` | Resultado 3a | Amortecimento Silk, Amplitude das Oscilações na Recombinação, escala linear. Calcula $r_{s}(\eta_\star)$ e $k_D(\eta_\star)$ por integração numérica completa. |
| `Resultado 04-ASSE(Escala Log).ipynb` | Resultado 3b | Amortecimento Silk, Supressão Exponencial, em escala log-log, evidenciando a estrutura completa de nós e picos. |
| `Resultado05-VOSBDCM.ipynb` | Resultado 4 | Velocity Overshoot e Sinal BAO na Distribuição de Matéria: defasagem de $\pi/2$ entre o sinal da RCF ($\cos kr_s$) e o sinal BAO na velocidade bariônica ($\sin kr_s$). |
| `Resultado06-FTT(k)(Escala Log-Log).ipynb` | Resultado 5 | Função de Transferência $T(k)$ completa (Eisenstein & Hu, 1998), em escala log-log, isolando as OABs da envoltória suave. |
| `Resultado07-EPLMDR.ipynb` | Resultado 6 | Espectro de Potências Linear da Matéria em Diferentes Redshifts, com normalização derivada da equação de Poisson e evolução via fator de crescimento $D_+(z)$. |

> Nota: a numeração dos arquivos (01 a 07) segue a ordem sequencial do
> repositório; a numeração "Resultado no TCC" (1, 2, 3a, 3b, 4, 5, 6)
> segue a numeração usada no texto do TCC, onde o amortecimento de
> Silk é apresentado em duas subseções (3a e 3b) a partir da mesma
> base numérica.

## Parâmetros cosmológicos

Todos os notebooks utilizam os parâmetros fiduciais do modelo
$\Lambda$CDM do Planck 2018: $\Omega_bh^2=0{,}0224$,
$\Omega_ch^2=0{,}120$, $\Omega_m=0{,}315$, $h=0{,}674$,
$n_s=0{,}965$, $\ln(10^{10}A_s)=3{,}044$, $z_*=1090$, $z_d=1060$,
$z_\mathrm{eq}=3400$, consistentes com a Tabela de parâmetros da
Metodologia do TCC.

## Requisitos

```
python >= 3.9
numpy
scipy
matplotlib
```

Instalação rápida:

```bash
pip install numpy scipy matplotlib
```

## Como executar

Cada notebook é independente e pode ser executado isoladamente (via
Jupyter Notebook, JupyterLab, Google Colab ou VS Code). Ao ser
executado, cada um imprime os valores numéricos calculados e a
respectiva verificação quantitativa (comparação com Planck 2018 e/ou
Eisenstein & Hu 1998), e salva a figura correspondente em `.png` e
`.pdf`.

## Citação

Se este código for útil para seu trabalho, ou caso deseje referenciá-lo,
utilize a citação abaixo:

```
SOUZA, Johnatans Neves. Códigos dos Resultados: Ondas Sonoras
Congeladas no Tempo: A RCF Como Régua Cósmica. Zenodo, 2026.
DOI: 10.5281/zenodo.22217922.
Disponível em: <https://doi.org/10.5281/zenodo.22217922>.
```

## Autor

Johnatans Neves Souza, Trabalho de Conclusão de Curso em Física, 2026.
