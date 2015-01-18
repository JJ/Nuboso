Nuboso
======

Nuboso con posibilidad de despliegue: computación nube en un enfoque
práctico. Un super-repositorio que contiene como submódulos las partes
de SaaS, desarrollo basado en pruebas, PaaS e IaaS (cuando la termine).

##Instrucciones

El repo usa diferentes submódulos, que son los que contienen en realidad el texto de cada uno de los capítulos. Eso quiere decir que se tiene que descargar de forma recursiva, en vez del habitual `git clone`:

	$ git clone --recursive https://github.com/JJ/Nuboso.git


Tras descargar el repo de la forma habitual, habrá que hacer

	$ git submodule foreach git pull               

si se ha hecho cambio en alguno de los subrepositorios. Y a partir de ahí, tras instalar `pandoc` con

	sudo apt-get install pandoc

se ejecuta 

	./md2epub

que genera un epub a partir de todos los capítulos en el mismo directorio llamado `nuboso.epub`. 

##¿Problemas? ¿Sugerencias?

Hazlo en [los *issues*](http://github.com/JJ/Nuboso/issues). Todos los parches y cambios se agradecerán y añadirán a la lista de agradecimientos del libro. 
