<div align="center">

![Editor](https://img.shields.io/badge/Editor-VSCode-blue?style=flat-square&logo=visual-studio-code&logoColor=white&style=flat)
![Projeto](https://badgen.net/badge/Projeto/Finished/green)
![GIT](https://badgen.net/badge/Git/ON/green?icon=github)
<!-- trocar o nome do repositório para atualizar -->
[![Profile last updated](https://img.shields.io/github/last-commit/verasdan/testejs?label=Last%20updated&style=flat)](https://github.com/verasdan/testejs/commits)

</div>

___

## Teste
Utilizando a lingagem JavaScript para manipular alguns elementos dentro da pagina HMTL. Foi utilizado esse script inicial para realizar alguns testes e por em prática a linguagem.

    <script>
    function acendeLampada(){
        document.getElementById("luz").src = "_imagens/lampada-acesa.jpg";
    }

    function apagaLampada(){
        document.getElementById("luz").src = "_imagens/lampada-apagada.jpg";
    }

    function quebraLampda(){
        document.getElementById("luz").src = "_imagens/lampada-quebrada.jpg";
    }

    </script>

<br>

foi utilizado 3 imagens para este teste.

![lampada-apagada](_imagens/lampada-apagada.jpg)
![lampada-acesa](_imagens/lampada-acesa.jpg)
![lampada-quebrada](_imagens/lampada-quebrada.jpg)

<br>

___

## Melhorando o codigo

Foi feita uma melhora no codigo para uma melhor compreensão e leitura do mesmo. Nessa parte foi utilizada o if para identificar a mudança de cada elemento.

    var quebrada = false;
    function mudaLampada(tipo){
        if (tipo == 1){
            arquivo = "_imagens/lampada-acesa.jpg";
        }

        if (tipo == 2){
            arquivo = "_imagens/lampada-apagada.jpg";
        }

        if (tipo == 3){
            arquivo = "_imagens/lampada-quebrada.jpg";
            
        }
        
        if (!quebrada){
            document.getElementById("luz").src = arquivo;
            if (tipo == 3){
                quebrada = true;
            }
        }

<br>

___

## Melhor solução

Para finalizar e ter um redimento no código foi melhorado e o final foi esse utilizando concatenação.

    var quebrada = false;
    function mudaLampada(tipo){
        
        if (!quebrada){
            document.getElementById("luz").src = "_imagens/" + tipo + ".jpg";
            if (tipo == 'lampada-quebrada'){
                quebrada = true;
            }
        }
        
    }

<br>

___

<br>
<!-- GitHub Contributors -->
<div align="center">

GitHub Contributors
<!-- Trocar o nome do repositório para atualizar -->
![GitHub Contributors Image](https://contrib.rocks/image?repo=verasdan/testejs)


</div>

___

<div align="center"><br>

![Profile Views](https://komarev.com/ghpvc/?username=verasdan)
![](https://badges.pufler.dev/visits/verasdan/verasdan?color=black&logo=github&style=flat-square)

[![Twitter Followers](https://badgen.net/twitter/follow/veras_dan)](https://twitter.com/veras_dan)
</div>