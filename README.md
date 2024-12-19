# Funções Utilizadas


## DAX
-Excluído e utilizado o SUMX
```bash
Total = f_Itens_Pedidos[Preço Venda]*f_Itens_Pedidos[Preço Venda]
```

## DAX
```bash
Cor-Ano = IF([Total-Realizado]<[Total-Realizado-Ano-Anterior],"#FF1010","#118DFF")
```

## SUMX e RELATED
```bash
Total-Previsto = SUMX(f_Itens_Pedidos,f_Itens_Pedidos[Qtde.]*RELATED(d_Produtos[Preço base]))
```

## SUMX
```bash
Total-Realizado = SUMX(f_Itens_Pedidos,f_Itens_Pedidos[Preço Venda]*f_Itens_Pedidos[Qtde.])
```

## SAMEPERIODLASTYEAR
```bash
Total-Realizado-Ano-Anterior = CALCULATE([Total-Realizado],SAMEPERIODLASTYEAR(d_calendario[Date]))
```

# Alterar a Fonte de Dados no Power BI Desktop

Para acessar os dados do arquivo, é necessário definir o caminho do banco de dados. Você pode alterar essa configuração nesta opção;
<p align="left">
  <img src="https://github.com/user-attachments/assets/602a5bae-ea0c-4483-8036-84118c49e986"alt="Captura de tela 2024-12-19 180410"width="250">
</p>

Após alterar o caminho do banco de dados, você deverá atualizar o Power BI para que ele carregue os dados;
<p align="left">
  <img src="https://github.com/user-attachments/assets/1fc53524-e9a0-42d8-bc76-6dc23eea9a45"alt="Captura de tela 2024-12-19 180613"width="150">
</p>
