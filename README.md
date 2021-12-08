# icon-and-name
scharc korar icon and 3. icom import
import 'package:flutter/material.dart';
void main()=> runApp(HomePage());
class HomePage extends StatefulWidget{
  @override
  _HomePageState createState() => _HomePageState();
}
class _HomePageState extends State<HomePage> {
  @override
  Widget build(BuildContext) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        appBar: AppBar(
          backgroundColor: Colors.deepOrange,
          title: Text("JIBON SHOP"),
          actions: <Widget> [
            new IconButton(onPressed: null, icon: Icon(Icons.search,color: Colors.white,))
          ],
        ),
        drawer: new Drawer(
          child: new ListView(
            children: <Widget> [
              new UserAccountsDrawerHeader(
                  accountName: Text("JIBON"),
                  accountEmail: Text("mdzibonranabd.com"),
                currentAccountPicture: GestureDetector(
                  child: new CircleAvatar(
                    backgroundColor: Colors.cyanAccent,
                    child: Icon(Icons.person, color: Colors.orange,),
                  ),
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
