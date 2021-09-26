# contact_list_drawer
import 'package:flutter/material.dart';

class ContactList extends StatelessWidget {
  // const ContactList({ Key? key }) : super(key: key);

  // List contact = [
  //   "+85225665",
  //   "630452055",
  //   "692305885024",
  //   "52358632"
  // ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("ListView & ListTile"),
        //leading: Icon(
        //Icons.menu,
        // color: Colors.white,
      ),
      drawer: Drawer(
        child: Column(
          children: [
            Stack(
              children: [
                Image.asset("assets/land_crusier.jpg"),
                Positioned(
                  left: 20,
                  top: 20,
                  child: Column(
                    crossAxisAlignment: CrossAxisAlignment.start,
                    children: [
                      CircleAvatar(
                        radius: 28,
                        backgroundImage: AssetImage("assets/poor_man.png"),
                      ),
                      Text(
                        "sujjada Zabin",
                        style: TextStyle(color: Colors.white, fontSize: 24),
                      ),
                      Text(
                        "sujjadazabin@gamil.com",
                        style: TextStyle(color: Colors.white, fontSize: 14),
                      ),
                    ],
                  ),
                ),
                // Positioned(
                //   left: 20,
                //   top: 80,
                //   child: Text(
                //     "sujjada Zabin",
                //     style: TextStyle(color: Colors.white, fontSize: 24),
                //   ),
                // ),
                // Positioned(
                //   left: 20,
                //   top: 110,
                //   child: Text(
                //     "sujjadazabin@gamil.com",
                //     style: TextStyle(color: Colors.white, fontSize: 14),
                //   ),
                // )
              ],
            )
          ],
        ),
      ),
      body: ListView.separated(
        separatorBuilder: (BuildContext context, int index) {
          return Divider(
            thickness: 1,
            height: 0,
            color: Colors.red,
          );
        },
        itemCount: 50,
        itemBuilder: (BuildContext context, int index) {
          return ListTile(
            // tileColor: Colors.teal,
            onTap: () {},
            leading: CircleAvatar(
              radius: 40,
              child: Icon(Icons.person),
            ),
            title: Text("+820296225666"),
            subtitle: Text("Flutter Devloper"),
            trailing: Icon(Icons.arrow_forward_ios),
          );
        },
      ),
    );
  }
}



new

import 'package:flutter/material.dart';

class ContactList extends StatelessWidget {
  // const ContactList({ Key? key }) : super(key: key);

  // List contact = [
  //   "+85225665",
  //   "630452055",
  //   "692305885024",
  //   "52358632"
  // ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text("ListView & ListTile"),
        //leading: Icon(
        //Icons.menu,
        // color: Colors.white,
      ),
      drawer: Drawer(
        child: Column(
          children: [
            Stack(
              children: [
                Image.asset("assets/land_crusier.jpg"),
                Positioned(
                  left: 20,
                  top: 20,
                  child: Column(
                    crossAxisAlignment: CrossAxisAlignment.start,
                    children: [
                      CircleAvatar(
                        radius: 28,
                        backgroundImage: AssetImage("assets/poor_man.png"),
                      ),
                      Text(
                        "sujjada Zabin",
                        style: TextStyle(color: Colors.white, fontSize: 24),
                      ),
                      Text(
                        "sujjadazabin@gamil.com",
                        style: TextStyle(color: Colors.white, fontSize: 14),
                      ),
                    ],
                  ),
                ),
              ],
            ),
            ListTile(
              onTap: () {},
              leading: Icon(
                Icons.music_note,
                color: Colors.grey,
              ),
              title: Text(
                "Music notebook",
              ),
            ),
            ListTile(
              onTap: () {},
              leading: Icon(
                Icons.settings,
                color: Colors.grey,
              ),
              title: Text(
                "Setting",
              ),
            ),
            ListTile(
              onTap: () {},
              leading: Icon(
                Icons.storage,
                color: Colors.grey,
              ),
              title: Text(
                "My file",
              ),
            )
          ],
        ),
      ),
      body: ListView.separated(
        separatorBuilder: (BuildContext context, int index) {
          return Divider(
            thickness: 1,
            height: 0,
            color: Colors.red,
          );
        },
        itemCount: 50,
        itemBuilder: (BuildContext context, int index) {
          return ListTile(
            // tileColor: Colors.teal,
            onTap: () {},
            leading: CircleAvatar(
              radius: 40,
              child: Icon(Icons.person),
            ),
            title: Text("+820296225666"),
            subtitle: Text("Flutter Devloper"),
            trailing: Icon(Icons.arrow_forward_ios),
          );
        },
      ),
    );
  }
}
