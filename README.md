# Analises_de_amostras

Para determinar o nível de expressão das KATs e KDACs em cada
amostra de cada experimento, usamos como parâmetro RPKM (Reads Per Kilo
base per Million mapped reads), que vai considerar o número de “reads” geradas
para cada gene em cada experimento e também o tamanho de cada gene. Para
obter o RPKM de cada gene, seguimos a seguinte equação:


## Cálculo de RPKM e Log2RPKM

### Passo 1: Calcular RPM (Reads Per Million)


$$
\text{RPM} = \left( \frac{\text{Número de reads do gene}}{\text{Número total de reads}} \right) \times 1.000.000
$$

### <br/>Passo 2: Calcular RPKM (Reads Per Kilobase Million)

$$
\text{RPKM} = \frac{\text{RPM do gene}}{\text{tamanho do gene (nt)}} \times 1.000
$$

### Passo 3: Calcular Log2RPKM

$$
\log_2\text{RPKM} = \log_2(\text{RPKM}) 
$$

Esse tipo de análise que empregamos serviu para normalizar os dados
entre as amostras eliminando vieses técnicos em dados sequenciados ou ajustar
fatores que possam causar variações no nível de expressão gênica, alterando o
resultado final. Normalizando as amostras com Log2RPKM é possível fazer uma
comparação mais precisa da expressão gênica. Todos os dados obtidos nesta
etapa foram plotados em gráficos para facilitar a visualização e as análises
comparativas entre as amostras, por exemplo, amostra de paciente infectado vs
não-infectado.
