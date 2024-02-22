# Formato padrão de telefone para formulariom 

feito para que seu formulario fique mais legivel

como manipular o numero de telefone para deixar com formato legivel



![image](https://github.com/Rafael-Teles-Alves/formato-Telefone-Formulario/assets/94096413/678ebe42-7f72-45dd-9fe4-7c18c0930a7a)

#  Nosso HTML fica assim! 🌟

    <!-- Formulário HTML -->
    <input type="text" id="phoneInput" placeholder="Digite o número de telefone">
    <button onclick="transformPhoneNumber()">Transformar</button>


# Agora vamos para o nosso JavaScript! 🚀

    <!-- Script JavaScript -->
    <script>
        // Vamos pegar os dados e transformar em valor antes de tudo
        function transformPhoneNumber() {
            var phoneInput = document.getElementById("phoneInput");
            var formattedPhone = transformPhone(phoneInput.value);
            phoneInput.value = formattedPhone;
        }
    
        function transformPhone(phone) {
            // Remove caracteres não numéricos do número de telefone
            phone = phone.replace(/\D/g, '');
    
            // Formatar o número de telefone para (XX) XXXX-XXXX
            var formattedPhone = '(' + phone.substring(0, 2) + ') ' + phone.substring(2, 6) + '-' + phone.substring(6, 10);
            return formattedPhone;
        }
    </script>

# Nesse caso, mesmo que nosso usuário digite somente os números, 

![image](https://github.com/Rafael-Teles-Alves/formato-Telefone-Formulario/assets/94096413/de4ef129-48b1-4f51-a98b-4ff31bab50bc)


JavaSript faz o tratamento para que o código não saia errado. 😉

![image](https://github.com/Rafael-Teles-Alves/formato-Telefone-Formulario/assets/94096413/716213ed-4e26-4abf-99c7-b54f09741fd1)


