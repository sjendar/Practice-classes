# Practice-classes
<!DOCTYPE html>
<body>
    <h2 id="title">Classes: The Basics</h2>
    <script type="text/javascript">
        /*
        class -> Object
        
        Instance Properties: What they have
        - name
        - age
        - height

        Instance Methods: What they do 
        - talk
        - run
        - jump
        */
       class Rectangle {
        //setup
        constructor (_width, _height, _color) {
            console.log("The rectangle is being created");
            this.width =  _width;
            this.height = _height;
            this.color = _color;

        }
        getArea () {
            return this.width * this.height;
        }
        printDescription() {
            console.log( 'I am a rectangle of ${this.width} x ${this.height} and I am ${this.color}  ')
        }
       }

       let myRectangle1 = new Rectangle(5, 3, "blue");
       let myRectangle2 = new Rectangle(10, 5, "red");

       myRectangle2.printDescription();

       console.log(myRectangle1.getArea());
       console.log(myRectangle2.getArea());



    </script>
</body>
