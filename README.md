

Tuotekuvasto app käyttää arkkitehtuurinaan Model-View-Controller (MVC) -mallia.
Model sisältää datan, jota ohjelma käyttää,
controller sisältää älyn, jolla dataa esitetään, muokataan ja haetaan,
view vastaa näkymistä, joissa data näytetään.

Model:
Applikaation testidata löytyy wwwroot:in tiedostosta products.json.
Model Product.cs sisältää Product class:n jota käytetään products.json:n datan muuntamisessa olioiksi.

Controller:
Controllerina toimiva HomeController.cs, lukee datana toimivan json-tiedoston ja välittää käännetyn ja deserialisoidun jsonin
Product olioiden listana metodissa GetProducts().

View:
HomeControllerin Product() -metodi kutsuu GetProducts() metodia ja käyttää sen palauttamaa listaa datana Product View:ssä.
Product View esittää applikaation testidatan ruudukkonäkymänä Product-olioista.

Ohessa kuvakaappaus MVC-mallin rakenteesta
![image](https://github.com/user-attachments/assets/19fd21db-10bb-4286-8957-5fba338da2d8)
Lähde: https://www.freecodecamp.org/news/the-model-view-controller-pattern-mvc-architecture-and-frameworks-explained/




