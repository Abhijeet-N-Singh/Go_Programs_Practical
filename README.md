This is an practical on Go Programming Language !

1) Write a Golang program that defines a struct and
   methods for calculating the area of a rectangle.
Answer code-


package main

import "fmt"

// Define a struct
type Rectangle struct {
	Length float64
	Width  float64
}

// Method to calculate area of a rectangle
func (r Rectangle) calculateArea() float64 {
	return r.Length * r.Width
}

func main() {
	// Creating an instance of Rectangle
	rect := Rectangle{Length: 5, Width: 3}

	//  Call method to calculate area
	area := rect.calculateArea()

	fmt.Printf("Rectangle Area: %.2f\n", area)
}
