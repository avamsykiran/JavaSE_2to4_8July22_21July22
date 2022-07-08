Java SE
------------------------------------------

    Presuming
            are already aware of:
                History
                Evolution
                Characteristics
                Data Types
                Variables
                Control Structures
                Operators
                Arrays

    Objectives
                OOPs
                java.lang   Standard Classes, Wrappr Classes, Exceptions, Multi-Theading
                java.time   Date Time Api
                java.util   Generics, Collections, Scanner, Random, Functional Interfaces, Lambda Expressions, Streams API
                java.io,
                java.nio    IO Streams
                java.sql    JDBC

    Lab Setup
                Eclispe IDE
                JDK 8
                MySQL

    Object Oriented Programming

                Class and Object

                        class is a user defiend data type to represent an entity
                            using Fields to represent the properties
                            and Methods to represent the behaviours

                        object is a varaible of class type.

                Encapsulation

                        is the process of data hiding. 

                        private
                        protected
                        public
                        default

                        setters and getters

                        'static' keyword
                        'this' keyword

                        constructor     is a special method that gets invoked as and when an object is allocated.
                                        is to initialize the valeus to the fields

                                        1. the construtor must have the same name as that of the class
                                        2. the constuctor do not return any value even not void.
                                        3. coinstructors can not be static.

                                        default constructor
                                        parmatrized constructor
                                        copy constructor

                        public class Circle {
                            private static double PI=3.14; //class variable
                            private double radius; //instacne -variables

                            public Circle(){
                                this.radius=0;
                            }

                            public Circle(double radius){
                                this.radius = radius;
                            }

                            public Circle(Circle c){
                                this.radius = c.radius;
                            }

                            public void setRadius(double radius){
                                this.radius=radius;
                            }

                            public double getRadius(){
                                return this.radius;
                            }

                            public boolean isGreaterThan(Circle c){
                               return this.radius > c.radius;
                            }

                            public static Circle add(Circle c1,Circle c2){
                                Circle c3 = new Cirlce();
                                c3.radius = c1.radius+c2.radius;
                                return c3;
                            }
                        }

                            Circle c1 = new Circle();
                            c1.setRadius(90);
                            Circle c2 = new Circle(190);
                            Circle c3 = new Circle(c1);

                            System.out.println(c2.isGreaterThan(c3));
                            System.out.println(c1.isGreaterThan(c2));

                            Circle c4 = Circle.add(c2,c3);


                Inheretence


                Polymorphisim
                Abstraction
    

    