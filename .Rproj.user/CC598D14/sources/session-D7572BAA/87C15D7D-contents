instrucao <- c("fundamental", "fundamental", "fundamental", "medio", 
               "fundamental",
               "fundamental","fundamental", "fundamental", "medio", "medio", 
               "medio","fundamental", "medio", "fundamental", "medio", "medio", 
               "medio", "fundamental",
               "superior", "medio", "medio", "medio", "fundamental", 
               "superior", "medio", 
               "medio", "fundamental", "medio", "medio", "medio", "superior",
               "medio", 
               "superior", "superior","medio", "superior")

regiao <- c("interior", "capital", "capital", "outra", "outra", "interior",
            "interior", "capital", "capital", "outra", "interior", "capital",
            "outra", "outra", "interior", "outra", "capital", "outra", 
            "interior", "interior", "outra", "capital", "outra", "outra",
            "interior", "outra", "outra", "interior", "interior", "capital",
            "outra", "interior", "capital", "capital", "capital", "interior")

salario <- c(4.00, 4.56, 5.25, 5.73, 6.26, 6.66, 6.86, 7.39, 7.59, 
             7.44, 8.12, 8.46, 8.74, 8.95, 9.13, 9.35, 9.77, 9.80,
             10.53, 10.76, 11.06, 11.59, 12.00, 12.79, 13.23, 
             13.60,13.85,14.69,14.71,15.99,16.22,16.61,17.26,
             18.75,19.40,23.30)


anos <- c(26,32,36,20,40,28,41,43,34,23,33,27,37,44,30,38,31,
          39,25,37,30,34,41,26,32,35,46,29,40,35,31,36,43,33,48,42)


dados <- data.frame(instrucao, regiao, salario, anos)

table(dados$instrucao, dados$regiao)

prop.table(table(dados$instrucao, dados$regiao))

esquisser(dados)



library(ggplot2)

ggplot(dados) +
 aes(x = regiao, y = salario) +
 geom_boxplot(fill = "#72517A") +
 labs(x = "Região", y = "Salário") +
 theme_minimal()
library(ggplot2)

ggplot(dados) +
 aes(x = instrucao, y = salario) +
 geom_boxplot(fill = "#E8D950") +
 labs(x = "Instrução", 
 y = "Salário") +
 ggthemes::theme_hc()
ggplot(dados1) +
 aes(x = salario, y = anos) +
 geom_point(shape = "bullet", size = 3.05, colour = "#112446") +
 labs(x = "Salário", y = "Anos", title = "Diagrama de Dispersão") +
 ggthemes::theme_hc() +
 theme(plot.title = element_text(size = 17L, 
 hjust = 0.5))


ggplot(dados) +
 aes(x = instrucao, fill = regiao) +
 geom_bar(position = "dodge") +
 scale_fill_viridis_d(option = "viridis", 
 direction = 1) +
 labs(x = "Grau de Instrução", y = " ", title = "Relação entre Grau de Instrução e Região", 
 fill = "Região") +
 ggthemes::theme_hc() +
 theme(plot.title = element_text(size = 17L, face = "bold", 
 hjust = 0.5))

freq_table(instrucao)





summary(dados)
summary(dados$salario)













