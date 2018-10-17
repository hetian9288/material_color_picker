# Material ColorPicker

Color picker for Flutter, based on the Google Docs color picker.

![alt text](https://raw.githubusercontent.com/long1eu/material_color_picker/master/res/extras/demo.png)

## Getting Started

You can embed into your material app or use it on a Dialog like this:

    Future<Color> askedToLead() async => await showDialog(
        context: context,
        child: new SimpleDialog(
          title: const Text('Select color'),
          children: <Widget>[
            new ColorPicker(
              type: MaterialType.transparency,
              onColor: (color) {
                Navigator.pop(context, color);
              },
              currentColor: startColor,
            ),
          ],
        ),
      );

For help getting started with Flutter, view our online [documentation](http://flutter.io/).
