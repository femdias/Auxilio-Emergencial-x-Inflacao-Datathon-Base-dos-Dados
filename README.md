# Auxilio Emergencial x Inflacão - Datathon-Base-dos-Dados

Essa análise pretende analisar a correlação entre o aumento dos preços e a incidência do Auxílio Emergencial através da manipulação de dados publicamente disponíveis.

As bases utilizadas foram:

1 -Base de população estimada do IBGE extraida com o module de Python basedosdados.
2 -Base de PIB do IBGE de 2018 extraida com o module de Python basedosdados.
3 -Base do Auxílio Emergencial, com dados entre abril e agosto, extraida do BigQuery do Base dos Dados através do código:

        SELECT SUM(valor_beneficio), sigla_uf, id_municipio
        FROM basedosdados.br_mc_auxilio_emergencial.microdados
        GROUP BY sigla_uf, id_municipio

4 - Tabela do IPCA extraida pelo sistema Sidra do IBGE, de acordo comas marcações: https://sidra.ibge.gov.br/tabela/7060#/n7/all/n6/all/v/69/p/202012/c315/7169,7171,7173,7175,7176,7283,12222,47617/d/v69%202/l/v,c315,t+p/cfg/nt,


As bases de dados extraidas de fora do Python estão anexadas neste Repositório, junto com o código em Python e o painel.
