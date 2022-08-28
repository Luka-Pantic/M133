# Lern-Bericht
Luka Pantic

## Einleitung

Im Modul 133 haben wir JSF (Jakarta Server Faces) behandelt. JSF ist ein Web Application Framework, welches benutzt wird, um grafische Benutzeroberflächen (GUIS) für Webanwendungen zu erstellen. Genauergesagt ging es um das Sessionhandling. Ein Beispiel wären zum Beispiel Eingaben in ein Formular. 

## Was habe ich gelernt?

In diesem Modul habe ich gelernt, wie ich eine Eingabe an eine andere Seite mit oder ohne eigenen Controller weiterleiten kann.

## Beschreibung

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/69889967/186891491-5fb460e8-bffa-4b7c-b8fe-e360ac2a7ef5.gif)

post ohne eigenen Controller:

```

<h:commandButton value="POST ohne eigenen Controller" action="post.xhtml"/>

```


post mit eigenem Controller:

```
<h:commandButton value="POST mit eigenem Controller" action="#{helloController.weiterleitung}"/>

```
    public class HelloManagedBean {

    /**
     * Creates a new instance of HelloManagedBean
     */
    public HelloManagedBean() {
    }
    
    private String eingabe;

    public String getEingabe() {
        return eingabe;
    }

    public void setEingabe(String eingabe) {
        this.eingabe = eingabe;
    }
    
    ```
    public class HelloController {

    /**
     * Creates a new instance of HelloController
     */
    public HelloController() {
    }
    
    public String weiterleitung(){
        return "post.xhtml";
    }
    }
    ```
    
    ![Screenshot 2022-08-28 212521](https://user-images.githubusercontent.com/69889967/187091108-d391741b-7872-41a0-bc45-e796c8777435.png)


## Verifikation

✍️ Erklären Sie kurz und bündig, inwiefern die von Ihnen verwendeten Medien zeigen, was Sie gelernt haben.

# Reflektion zum Arbeitsprozess

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
