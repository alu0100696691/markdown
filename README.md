INSTALACIÓN RVM/RUBY Y GIT
==========================

**Autor:** *José Antonio Rodríguez Leandro*  

**Fecha:** *11 Septiembre 2014*

* Instalando RVM


	A la hora de instalar esta herramienta, nos aseguramos que el usuario no  fuera administrador y 
mucho menos root, ya que mi intensión es que la instalación no fuera multiusuario. 
Para instalar RVM es necesario disponer de "curl", en mi caso ya disponía de esta herramienta, por lo que me dispuse a instalar directamente ejecutando el siguiente comando:

`$ \curl -#L https://get.rvm.io | bash -s stable --autolibs=3 --ruby`

![Imagen, instalando RVM](img/rvm1.png?raw=true "Instalando RVM")

	Luego se modifico el fichero *~/.bash_profile*, con el codigo:
	
	`echo "source $HOME/.rvm/scripts/rvm" >> ~/.bash_profile`

![Imagen, archivo .bash_profile](img/rvm3.png?raw=true "Modificando bash_profile")

* Instalando Ruby
 

	Con el comando anterior, la última versión estable de ruby es instalada. Pero para añadir una versión con mas tiempo en el mercado, instale la ruby **1.9.3**

```
rvm install 1.9.3
rvm use 1.9.3 
```
![Imagen, instalando Ruby](img/rvm4.png?raw=true "Instalando Ruby")


* Git y las Gemas Sinatra y twitter
 

	El último paso es la instalación de Git, el cual ya estaba instalado en el sistema, así como las gemas *sinatra* y *twitter*.

Instalar git es muy sencillo:

 `$ apt-get install libcurl4-gnutls-dev libexpat1-dev gettext \ libz-dev libssl-dev`
 
 `$ apt-get install git`

Al igual que las gemas:

 `gem install sinatra`
 
 `gem install twitter`

![Imagen, instalando Sinatra](img/rvm7.png?raw=true "Instalando Sinatra")
![Imagen, instalando twitter](img/rvm8.png?raw=true "Instalando twitter")

	
FUENTES:

![Enlace: instalar RVM/ruby](http://rvm.io/rvm/install "Instalar RVM/ruby")

![Enlace: instalar Git](http://git-scm.com/book/es/Empezando-Instalando-Git "Instalar Git")

![Enlace: instalar sinatra](https://rubygems.org/gems/sinatra "Instalar sinatra")

![Enlace: instalar twitter](https://rubygems.org/gems/twitter "Instalar twitter")






