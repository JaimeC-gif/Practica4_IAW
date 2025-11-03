UD02 - Pràctica 04

Curs 2025-2026
![ref1]![ref2]![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.003.png)![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.004.png)

<a name="pràctica_4%25253a_phpmyadmin"></a>**Pràctica 4: phpmyadmin**

# <a name="objectiu"></a>**Objectiu**

- Instal·lar, assegurar i configurar phpMyAdmin en un servidor Ubuntu.
- Protegir PhpMyAdmin contra accessos no autoritzats.
- Automatitzar la instal·lació i configuració de phpMyAdmin mitjançant scripts de Bash.

# <a name="tasques_a_fer"></a>**Tasques a fer**

## **Instal·lació de PhpMyAdmin**
- Instal·la phpMyAdmin juntament amb les extensions PHP necessàries (php-mbstring, php-zip, php-gd, php-json, php-curl).

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.005.png)






- Configura phpMyAdmin perquè funcione amb nginx.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.006.png)![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.007.png)
##
##
## **Permetre l’Accés per Contrasenya del root de MySQL**
- Canvia el mètode d’autenticació de l’usuari root de MySQL d’auth\_socket a caching\_sha2\_password o mysql\_native\_password.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.008.png)






- Verifica els mètodes d’autenticació utilitzats per cadascun dels usuaris.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.009.png)







## **Configuració de l’Accés per Contrasenya per a un Usuari Dedicat de MySQL**
- Crea un nou usuari de MySQL amb una contrasenya segura.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.010.png)



- Dona-li al usuari els privilegis apropiats per gestionar les bases de dades a través de phpMyAdmin.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.011.png)


## **Assegura la Instància de phpMyAdmin**
- Crea un fitxer .htpasswd per emmagatzemar les credencials d’usuari i contrasenya.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.012.png)



- Modifica la configuració del lloc per aplicar l’accés per usuari i contrassenya.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.013.png)









- Reinicieu nginx per aplicar els canvis.

  ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.014.png)

![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.015.png)![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.016.png)Assegureu-vos de seguir bones pràctiques de seguretat a cada pas. No inclogueu con- trasenyes reals a les captures de pantalla o al document. El document ha d’estar ben organitzat i fàcil de seguir.

## **Com Lliurar**
Hauràs de crear un repositori a GitHub amb el nom de la pràctica i la descripció de la mateixa. El repositori ha de tenir el contingut següent:

![ref3]

IAW - 2ASIX	[1/](#_bookmark0)






<a name="_bookmark0"></a>Una **documentació tècnica** al vostre repositori de Github, i publicat a Github Pages amb la descripció de tots els passos que s’han dut a terme.

- Els passos detallats que vas seguir per completar cadascun dels requisits.
- Instal·lació i configuració de phpMyAdmin.
- Configuració d’autenticació i mètodes d’autenticació de MySQL i Nginx.
- Els scripts de Bash que s’han utilitzat per automatitzar la instal·lació i configuració de PhpMyAd- min.
- Captures de pantalla demostratives dins de la documentació.

A més del contingut anterior pot ser necessari crear altres fitxers de configuració. A continuació es mostra un exemple de com pot ser lestructura del repositori:

1

2

3

4

5

6

7

8

.-¬

|- README.md

|- conf

-¬

|- site\_phpmyadmin

|- scripts -¬

|- .env

|- install\_lemp.sh

|- install\_phpmyadmin.sh
## ![](Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.018.png)**Scripts de Bash**
El directori scripts ha d’incloure els fitxers següents:

- **.env**: Aquest fitxer conté totes les variables de configuració que s’utilitzaran als scripts de Bash.
- **install\_lemp.sh**: Script de Bash amb l’automatització del procés d’instal·lació de la pila LEMP.
- **install\_phpmyadmin.sh**: Script de Bash amb l’automatització del procés de creació i configura- ció d’instal·lació i securització de phpMyAdmin.

# <a name="recursos"></a>**Recursos**

- [Documentación de phpMyAdmin](https://www.phpmyadmin.net/docs/)
- [Documentación de MySQL](https://dev.mysql.com/doc/)
- [Documentación de NGINX](https://nginx.org/en/docs/)

![ref3]IAW - 2ASIX	[2/2](#_bookmark0)

[ref1]: Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.001.png
[ref2]: Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.002.png
[ref3]: Aspose.Words.3c225a72-eca6-4739-841e-ecdc5fa3400b.017.png
