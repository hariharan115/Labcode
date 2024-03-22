### Java Methods
```Java
public class Hello {
    public static void main(String[] args) {
        Hello activate = new Hello();
        activate.spotify_Methods();              // static to non static
        System.out.println("Hello World!");             
    }

    void spotify_Methods() {
        Hello activate1 = new Hello();           // non static to non static
        activate1.google_Methods();              
        System.out.println("Play On High On Love Song!");
    }

    void google_Methods() {
        Hello.book_Methods();                    // non static to static
        System.out.println("Hey Google!");
    }

    static void book_Methods() {
        Hello.gmail_methods();                   // static to static
        System.out.println("Java Fundamendals");
    }

    static void gmail_methods() {
        System.out.println("Inbox 4 messages!");
    }
}
```
### Parameters and arguments
```Java
public class Hello {

    public static void main(String[] args) {
        Hello activate = new Hello();
        activate.google_Methods();
        String songs = activate.spotify_Methods();
        System.out.println(songs);
        activate.whatApp_Methods(85, 4, "Hey there!");
        int All_mail = activate.gmail(40, 10);
        System.out.println(All_mail);
        
    }

    void google_Methods() {
        System.out.println("Hey Google!");       //no return, no arguments
    }

    String spotify_Methods() {
        return "Play On High On Love Song";      //with return, no arguments
    }

    void whatApp_Methods(int contacts, int chats, String message) {
        System.out.println("message: " + message);
        System.out.println("contacts: " + contacts);    //no return, with arguments
        System.out.println("chat: " + chats);
    }

    int gmail(int inbox, int send) {
        return inbox + send;                     //with return, arguments
    }
}
```
