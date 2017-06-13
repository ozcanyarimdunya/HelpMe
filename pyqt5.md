### Create an app's design.py file that you created via pyuic, import it into your project files.
### Create a class to test design.py
    
    import design # your design file created automatically from design.ui file (pyuic5 design.ui -o design.py)
    class ExampleApp(QtGui.QMainWindow, design.Ui_MainWindow):
        def __init__(self, parent=None):
            super(ExampleApp, self).__init__(parent)
            self.setupUi(self)
            
    if __name__ == '__main__':
        app = QtGui.QApplication(sys.argv)
        form = ExampleApp()
        form.show()
        app.exec_() # or sys.exit(app.exec_())
