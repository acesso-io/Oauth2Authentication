## Exemplo de utilização:

Com a LIB disponível no projeto, basta instanciar o objeto e utilizar os recursos disponíveis. 

Exemplo em C#:

`
Identity_Authenticator.Identity_Authenticator identity = new Identity_Authenticator.Identity_Authenticator();
            try
            {
                var token = identity.GetToken("https://identityhomolog.acesso.io/", @"`**Repositório onde se encontra a chave privada**`", "sdk_auth", "<TENANT_ID>");
                Console.Write(token);
            }
            catch (Exception Ex)
            {
                Console.Write(Ex);
            }
`

Neste exemplo o sistema irá realizar apenas uma chamada para a Plataforma, no ambiente de homologação, e receberá o Token ou um retorno de erro. 
