Instruções de como o parceiro pode utilizar SAS para compartilhar arquivos com a Allpoints.

 
Os dados recebidos pelo parceiro serão os seguintes:


**ENDPOINT**

https://partners.data.allpointstravel.com/ferrasa


**SAS**

sv=2020-04-08&si=2030&sr=c&sig=U%2BFlnBUFqdd0173ggI%2BwbNbCRmkAEUklK6S3Djn4uDI%3D

 
**URL DE TESTE**

https://partners.data.allpointstravel.com/ferrasa/?restype=container&comp=list&sv=2020-04-08&si=2030&sr=c&sig=U%2BFlnBUFqdd0173ggI%2BwbNbCRmkAEUklK6S3Djn4uDI%3D


ENDPOINT é a URL única do parceiro no compartilhamento de arquivos da Allpoints


SAS é a chave segura de acesso do parceiro e deve ser mantida em segurança. Só é possível acessar os dados do parceiro com a sua chave segura de acesso.


URL DE TESTE é um link que pode ser utilizado no navegador para testar se o Endpoint e o Sas estão funcionando corretamente.

Este Endpoint deve retornar status HTTP 200 OK. Qualquer outro status indica que existe algo errado.


Para o envio dos arquivos, é possível que seja efetuado manualmente ou pela Api do Storage.

O envio manual pode ser efetuado pela ferramenta Azure Storage Explorer.

O link abaixo detalha como obter, instalar e utilizar esta ferramenta oficial da Microsoft:

https://docs.microsoft.com/pt-br/azure/vs-azure-tools-storage-manage-with-storage-explorer?tabs=windows

A integração via Api de Storage pode ser feita utilizando requisições Http em qualquer linguagem.

O link abaixo detalha como manipular os Blobs(arquivos)

https://docs.microsoft.com/pt-br/rest/api/storageservices/service-sas-examples
