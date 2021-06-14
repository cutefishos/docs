# MenuBar

In the Cutefish desktop, you can add MenuBar in the app to display in the top of the desktop. 

![Screenshot](/_static/2021-06-14-appmenu.png)

## How to use?

Add import `Qt.labs.platform 1.0` in the head of `main.qml`

```qml
MenuBar {
    id: menuBar

    Menu {
        id: fileMenu
        title: qsTr("File")
    }

    Menu {
        id: editMenu
        title: qsTr("&Edit")
    }

    Menu {
        id: viewMenu
        title: qsTr("&View")
    }

    Menu {
        id: helpMenu
        title: qsTr("&Help")

        MenuItem {
            text: "About"
        }
    }
}
```

Related Link: [https://doc.qt.io/qt-5/qml-qt-labs-platform-menubar.html](https://doc.qt.io/qt-5/qml-qt-labs-platform-menubar.html)