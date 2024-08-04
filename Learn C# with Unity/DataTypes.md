# Data Types

Discover C# data types and their usage with variables, such as integers, floats, strings, booleans, and arrays.

## Introduction
C# is a powerful programming language commonly used in game development, and Unity is a popular game engine that uses C# as its primary scripting language. In this lesson, we’ll explore some of the critical concepts and syntax of C# in Unity and provide examples and illustrations to help you understand the language.

## Integers
Integers store whole numbers in C#, and the `int` keyword represents them. Integers are commonly used in game development to describe scores, health points, and other numerical values.
```csharp
int health = 100;
```
In this example, we declare an integer variable `health` and assign it a value of `100`.

## Floating Point Numbers
Floating point numbers store decimal numbers in C# and the `float` keyword represents them. Floating point numbers are commonly used in game development to describe positions, rotations, and other 3D coordinates.

```csharp
float moveSpeed = 5.0f;
```
In this example, we declare a floating point variable `moveSpeed` and assign it a value of `5.0f`.

## Strings
Strings store text in C# and the `string` keyword represents them. Strings are commonly used in game development to display messages, dialogue, and text-based content.
```csharp
string playerName = "Player1";
```
In this example, we declare a string variable `playerName` and assign it a value of `"Player1"`.

## Booleans
Booleans store true or false values in C# and the `bool` keyword represents them. Booleans are commonly used in game development to describe whether a GameObject is active or inactive, whether the game is over, and other logical values.
```csharp
bool isGameOver = false;
``` 
In this example, we declare a boolean variable `isGameOver` and assign it a value of `false`.

## GameObjects
Unity uses the `GameObject` class to represent objects in the scene. GameObjects are the fundamental building blocks of a Unity scene and can contain components such as `Transform`, `MeshRenderer`, `Collider`, and `Scripts`. GameObjects can be created, modified, and destroyed during gameplay to create interactive and dynamic experiences.
```csharp
GameObject player = Instantiate(playerPrefab, new Vector3(0, 0, 0), Quaternion.identity);
```
Instantiate playerPrefab at (0, 0, 0) with no rotation

## Vectors
Unity uses the `Vector3` class to represent 3D vectors in the scene. Vectors are commonly used in game development to describe positions, rotations, and scales of GameObjects.
```csharp
Vector3 playerPosition = new Vector3(0, 0, 0);
```
In this example, we declare a Vector3 variable `playerPosition` and assign it a value of `(0, 0, 0)`.
## Quaternion
Unity uses the `Quaternion` class to represent rotations in the scene. Quaternions are commonly used in game development to describe rotations of GameObjects.
```csharp
transform.rotation = Quaternion.Euler(0, 90, 0);
```
Set the GameObject rotation to 90 degrees around the y-axis

## Arrays
Arrays store collections of elements in C# and the `[]` syntax represents them. Arrays are commonly used in game development to store multiple GameObjects, positions, and other data.
```csharp
GameObject[] enemies = new GameObject[10];
```
In this example, we declare an array of GameObjects `enemies` with a length of `10`.

## Enums
Enums define custom data types in C# and the `enum` keyword represents them. Enums are commonly used in game development to represent a set of related values, such as different player classes or game modes.
```csharp
public enum PlayerClass
{
    Warrior,
    Mage,
    Archer
}
```
In this example, we declare an enum `PlayerClass` with three values: `Warrior`, `Mage`, and `Archer`.

## Structs
Structs are similar to classes in C#, but they are used to store small, lightweight data types. Structs are commonly used in game development to represent simple data types, such as coordinates or colors.
```csharp
public struct Coordinate
{
    public float x;
    public float y;
    public float z;
}
```
In this example, we declare a struct `Coordinate` with three fields: `x`, `y`, and `z`.

## Summary
It’s important to choose the correct data type for a variable because it affects how the variable can be used and how much memory it will take up. For example, we cannot use a string variable to represent a player’s health because strings are used for text and health is a number.

Also, it is essential to use the correct suffix for floating point numbers, like `f` for `float` and `d` for `double`.