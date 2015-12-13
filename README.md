##Guia de instalação do ambiente para o uso do Calabash 2

###Requerimentos
1. Ruby: versão 1.9.3 ou superior
2. Android Studio
3. Xcode
4. Um computador mac - Caso vá desenvolver testes automatizados para o Android e iOS

###Instalando o Ruby através do RVM (Ruby Version Manager) 

Para usarmos o Calabash precisamos apenas do Ruby instalado na máquina. Porém convém instalarmos um gerenciador de versões do ruby na máquina, principalmente por que eventualmente podemos instalar versões conflitantes de gems na máquina e que pode vir a ser uma dor de cabeça.

Para evitar estes problemas usamos o RVM que gerencia versões diferentes do ruby instalado na máquina e os gems sets. Para instalar siga as instruções: [https://rvm.io/rvm/install](https://rvm.io/rvm/install)

Para ver todas as versões de rubies que podem ser instalados na máquina:
```
$rvm list known
```

Para instalar uma versão específica do ruby, ex:
```
$rvm install 2.2.1
```

Para verrificar a instalação digite:
```
$ruby -v
=> ruby 2.2.1p85 (2015-02-26 revision 49769) [x86_64-darwin14]
```

Para criar um gemset novo (completamente vazio, sem nenhuma gem instalada e portanto sem conflitos) basta digitar:
```
$ rvm gemset create calabash-gemset
```

para verificar as gemsets do sistama:
```
$rvm gemset list
gemsets for ruby-2.2.1 (found in /Users/msantini/.rvm/gems/ruby-2.2.1)
=> (default)
   calabash-gemset
   global
```
Podemos notar no output acima que a setinha indica que estamos usando o gemset default, ou seja, do sistema para selecionar a gemset que criamos basta executar:
```
$rvm gemset use calabash-gemset
=>Using ruby-2.2.1 with gemset calabash-gemset
```

Pronto, agora temos um ambiente pronto para a instalação do calabash-android e o calabash-ios

###Instalando o Android Studio


