# Relatorio (Passo a passo para resolução)

 Ao tentar abrir arquivo normalmente pelo excel, o texto ficou embaralhado com alguns caracteres especiais. Fechei o programa e reabri o mesmo em branco, escolhi a opção de *Dados → Obter Dados → De Arquivo → De Texto/CSV*.
Importado o arquivo, selecionei a opção de origem do arquivo para *65001: Unicode (UTF-8)*, separado por virgula e carreguei.

### **Removendo duplicata:**
Selecionei toda a tabela *(Ctrl+shift+ seta direita e Ctrl+shift+ seta baixo)*, marquei opção de tabela de design (opção canto superior direito), remover duplicatas. 

### **Padronizando datas:**
Selecionei coluna data. Na caixa de pesquisa do excel, procurei por formatar célula, data e escolhi o formato apropriado.

### **Corrigindo valores nulos:**
Para verificar se existiam células vazias, foi aplicado um filtro de condicional em que toda a tabela para verificar se havia células e que as mesmas fossem preenchidas com uma cor <span style="color:red;">(vermelho)</span> para melhor visualização do cliente, já que o mesmo não instruiu a tratativa a ser efetuada com esse tipo de problemática.
Para verificação da aba de preços, criei uma coluna com a formula *=VALOR([@Preço])* para que todo valor que estivesse fora do padrão numérico fosse identificado e se possível, corrigido. Valores confusos (com caracteres especiais ou letras misturadas aos números também foram repassados ao cliente afim de buscar a melhor tratativa).
Para contagem de células em branco e valores nulos apliquei filtro em cada coluna e formula *=Subtotal(a:b)*. Depois filtrei coluna por coluna, verificando cada valor e somei tudo no fim usando *=SOMA(a:b)*.

### **Conclusão**
Após cliente informar como deve ser tratado os dados que estão inconsistentes relatório final (resumido) será planejado.
