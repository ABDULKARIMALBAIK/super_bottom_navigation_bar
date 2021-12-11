# [super_bottom_navigation_bar](https://pub.dev/packages/super_bottom_navigation_bar/install)

Amazing powerful animated widget, it is useful for modern apps by displaying pro BottomNavigationBar with ViewPager.

Add Super BottomNavigationBar => Better UI/UX.


[![pub](https://img.shields.io/pub/v/super_bottom_navigation_bar?color=blue&label=pub&logo=flutter&style=flat-square)](https://pub.dev/packages/super_bottom_navigation_bar/install)
[![license](https://img.shields.io/github/license/ABDULKARIMALBAIK/super_bottom_navigation_bar?color=yellow&label=license&logo=github&style=flat-square)](https://pub.dev/packages/super_bottom_navigation_bar/install)
[![repo_size](https://img.shields.io/github/languages/code-size/ABDULKARIMALBAIK/super_bottom_navigation_bar?color=red&label=repo_size&logo=github&style=flat-square)](https://pub.dev/packages/super_bottom_navigation_bar/install)


# URLS



# Features

**Animation**

You can feel the animation with this package when tab is selected.

**Configurable Widget**

You can control any part of this widget backgroundColor , icons , size , type of animation , colors and more...

**Strong build**

The package is built with strong tests to make it trusted to developers

**Beautiful UI**

With this package you can make `POWERFUL` UI.



# Installing

Add this to your package's `pubspec.yaml` file:

```yaml
dependencies:
  super_bottom_navigation_bar: latest_version
```

Then import it :

```dart
import 'package:super_bottom_navigation_bar/super_bottom_navigation_bar.dart';
```

More details see [pub.dev](https://pub.dev/packages/super_bottom_navigation_bar/install).



# Usage

The `super_bottom_navigation_bar` package you can use it simply :



> :warning:: The `items` value must be `items >= 1`.
> :warning:: The `currentIndex` value must be `currentIndex >= 0 && currentIndex < items.length`.



**Simple Design**

```
      Scaffold(
              bottomNavigationBar: SuperBottomNavigationBar(
                currentIndex: 1,
                items: [
                  SuperBottomNavigationBarItem(),
                  SuperBottomNavigationBarItem(),
                  SuperBottomNavigationBarItem(),
                ],
                onSelected: (index){
                  print('tab $index');
                },
              ),
      ...........
          );
```


### URL1



**Normal Design**

```
      Color primaryColor = Colors.yellowAccent;
      ........
      Scaffold(
              bottomNavigationBar: SuperBottomNavigationBar(
                currentIndex: 1,
                items: [
                  SuperBottomNavigationBarItem(
                    unSelectedIcon: Icons.home_outlined,
                    selectedIcon: Icons.home,
                    splashColor: primaryColor,
                    borderBottomColor: primaryColor,
                    backgroundShadowColor: primaryColor,
                    selectedIconColor: primaryColor,
                    unSelectedIconColor: Colors.grey
                  ),
                  SuperBottomNavigationBarItem(
                      unSelectedIcon: Icons.favorite_border,
                      selectedIcon: Icons.favorite,
                      splashColor: primaryColor,
                      borderBottomColor: primaryColor,
                      backgroundShadowColor: primaryColor,
                      selectedIconColor: primaryColor,
                      unSelectedIconColor: Colors.grey
                  ),
                  SuperBottomNavigationBarItem(
                      unSelectedIcon: Icons.cloud_done_outlined,
                      selectedIcon: Icons.cloud_done,
                      splashColor: primaryColor,
                      borderBottomColor: primaryColor,
                      backgroundShadowColor: primaryColor,
                      selectedIconColor: primaryColor,
                      unSelectedIconColor: Colors.grey
                  ),
                ],
                onSelected: (index){
                  print('tab $index');
                },
              ),
          ...........
           );
      
```


### URL2



**Super Design**

```
      Scaffold(
              bottomNavigationBar: SuperBottomNavigationBar(
                currentIndex: 2,
                items: makeNavItems(),
                onSelected: (index){
                  print('tab $index');
                },
              ),
         .........
          );
      
      
      List<SuperBottomNavigationBarItem> makeNavItems() {
         return [
               SuperBottomNavigationBarItem(
                 unSelectedIcon: Icons.home_outlined,
                 selectedIcon: Icons.home_outlined,
                 size: 30,
                 backgroundShadowColor: Colors.red,
                 borderBottomColor: Colors.red,
                 borderBottomWidth: 3,
                 // highlightColor: Colors.red,
                 // hoverColor: ,
                 splashColor: Colors.red,
                 selectedIconColor: Colors.red,
                 unSelectedIconColor: Colors.red
               ),
               SuperBottomNavigationBarItem(
                   unSelectedIcon: Icons.search_outlined,
                   selectedIcon: Icons.search_outlined,
                   size: 30,
                   backgroundShadowColor: Colors.blue,
                   borderBottomColor: Colors.blue,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.blue,
                   selectedIconColor: Colors.blue,
                   unSelectedIconColor: Colors.blue
               ),
               SuperBottomNavigationBarItem(
                   unSelectedIcon: Icons.star_border_outlined,
                   selectedIcon: Icons.star_border_outlined,
                   size: 30,
                   backgroundShadowColor: Colors.yellowAccent,
                   borderBottomColor: Colors.yellowAccent,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.yellowAccent,
                   selectedIconColor: Colors.yellowAccent,
                   unSelectedIconColor: Colors.yellowAccent
               ),
               SuperBottomNavigationBarItem(
                   unSelectedIcon: Icons.done_outline_rounded,
                   selectedIcon: Icons.done_outline_rounded,
                   size: 30,
                   backgroundShadowColor: Colors.green,
                   borderBottomColor: Colors.green,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.green,
                   selectedIconColor: Colors.green,
                   unSelectedIconColor: Colors.green
               ),
               SuperBottomNavigationBarItem(
                   unSelectedIcon: Icons.person_outline,
                   selectedIcon: Icons.person_outline,
                   size: 30,
                   backgroundShadowColor: Colors.purpleAccent,
                   borderBottomColor: Colors.purpleAccent,
                   borderBottomWidth: 3,
                   // highlightColor: Colors.red,
                   // hoverColor: ,
                   splashColor: Colors.purpleAccent,
                   selectedIconColor: Colors.purpleAccent,
                   unSelectedIconColor: Colors.purpleAccent
               ),
             ];
      }
```


### URL3



# Widget Properties

**SuperBottomNavigationBar**


`items`

*List<SuperBottomNavigationBarItem>  (required)*

list of SuperBottomNavigationBarItem to show them in your BottomNavigationBar.



`currentIndex`

*int*

The tab to display.



`height`

*double*

Height of the BottomNavigationBar.



`backgroundColor`

*Color*

backgroundColor of BottomNavigationBar.



`curve`

*Curve*

The transition curve.



`duration`

*Duration*

The transition duration.
 
 
 
`padding`
 
 *EdgeInsets*
 
The padding surrounding the entire widget , You can use to adding floating effect.



`elevation`
 
 *double*
 
The elevation of the widget.



`onSelected`
 
 *ValueChanged<int>?*
 
Callback method , Return the index of the tab that was tapping.


---

