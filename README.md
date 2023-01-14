# -teste-DocX-C-

o arquivo esta compactado por motivos de tamanho

o arquivo é um web que le o arquivo do local especificado e o modifica e gera um novo arquivo

basta dentro do visual etudio executar o index no navegador de sua preferenci
ira abri uma pagina com apenas um link em azul
esse link te leva  ate o formulario para adicionar as informações
e com um botão ele irá gerar um novo arquivo.

para  configurar voce precisar ir no arquivo dominio e passar o local do arquivo que quer modificar isso na variavel caminho 
  exemplo caminho = @"C:\Users\guisc\Downloads\Nova pasta\testes\";

na variavel documento voce passa o nome do documento que será modificado
    exemplo (var documento = DocX.Load(caminho + "documento.docx"))
    voce só precisa passar o nome do arquivo no lugar do exemplo que esta "documento.docx"
  
  vou botar o documento do exemplo junto aqui pode uasr ele se quiser ou gerar outro só lembre que o programa só vai trocar 
   quando encontrar o padrao @nome , @cpf e @email.
e para trocar o nome do novo docuemnto basta trocar o nome no codigo onde aparece SAVEAS
exemplo documento.SaveAs(caminho + "Novo-documento.docx");
basta substituir "Novo-documento.docx" pelo nome que voce quiser
