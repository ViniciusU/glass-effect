# glass-effect

EVALUATE
SUMMARIZECOLUMNS(
'dCalendário'[Ano],
d_IES[Região],
d_IES[UF],
d_IES[Estado],
d_IES[Organização Acadêmica],
dimUnidade[Instituicao],
d_IES[Instituição (Nome)],
"Gastos Correntes por matrícula", [Gastos_Correntes_matricula],
"Gastos Totais", [Gastos Correntes | Gastos Totais],
"Gastos Correntes", [Gastos Correntes | Gastos Correntes],
"Inativos e Pensionistas", [Gastos Correntes | Inativos e Pensionistas],
"Investimentos e Inversões", [Gastos Correntes | Investimentos e Inversões Financeiras],
"Precatórios", [Gastos Correntes | Precatórios],
"Outros Custeios", [Gastos Correntes | Outros Custeios],
"Gastos de Pessoal", [Gastos Correntes | Pessoal]
)
ORDER BY
'dCalendário'[Ano] ASC,
d_IES[Região] ASC,
d_IES[UF] ASC,
d_IES[Estado] ASC,
d_IES[Organização Acadêmica] ASC,
dimUnidade[Instituicao] ASC,
d_IES[Instituição (Nome)] ASC
