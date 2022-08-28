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


![Screenshot 2022-08-28 212521](https://user-images.githubusercontent.com/69889967/187091192-a09f1c91-f25b-4a15-beb7-130d5ad309ed.png)

  


## Verifikation

1. In der Methode ohne den Controller wird einfach direkt auf die "post.xhtml" Seite verwiesen.
2. Bei der anderen Methode wird erst auf den HelloController verwiesen, mit der Methode "weiterleitung"
   an die "HelloManagedBean" weitergeleitet.
   
   

# Reflektion zum Arbeitsprozess

Bei diesem Arbeitsauftrag wurde zwar das Programm schon vorgegeben, doch man hat trotzdem einen guten Einblick in das Prinzip von
JSF bekommen können.

Ich hatte manchmal ein Paar Probleme beim Kompilieren des Programms, doch das Problem war meistens, dass das Falsche "JDK" ausgewählt war.

Im nächsten Modul sollte ich mich etwas mehr am Unterricht beteiligen und falls es wieder zum Distanzunterricht kommt mich etwas weniger ablenken lassen.
