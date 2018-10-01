AmplifyShaderFunctions
=======

![gif](http://i.imgur.com/OFjCw9w.gif) ![gif](http://i.imgur.com/296gdVp.gif)

My additionnal functions for shading in Unity, using *Amplify Shader* plugin.

AMPLIFY SHADER FUNCTIONS TYPES
-------------------

### Shader types
There is 5 types of functions made :

- Random : some functions for fast randomization with Float and Vec2.
- Shapes : some functions to help you create basic shapes (circle, square, triangle, rect, and with/without edges)
- Waves : some functions to help you making gradients ou lerp values from A to B with a precise wave shape.
- Transform : nodes to transform space and time. Can't do coffee at the same time.
- Other : wip functions without a type (like amod).

### Nodes usage
All nodes are designed the same way :
- 0-1 value mean 0 for nothing and 1 for max default value. ex : for a circle 0 for radius means an invisible cricle and 1 a big circle with edges touching the uvs.
- when an input "UVs" can be used, you need to add a node Texture Coordinate or a transformation of uvs.

SHAPES SPECIALS
-------------------

### Basic usage of Shape Circle
![gif](http://i.imgur.com/5ZmmCis.gif)
Most of shapes are designed on this first node. The pivot can change the center of the shape. UVs means a representation of space and can be used with Texture Coordinate. Radius means the size of the circle.

### Amod function
![gif](http://i.imgur.com/fq9BKtZ.gif)
Thanks to Flopine & Koltes, Amod function is a way for duplication shapes in a circle. It uses polar coordinates. For simplification : you don't duplicate the shape, you "duplicate" the space where the space will be created.

UPDATES
-------------------

### 2018-10-01
Add Transform type
Remove Rotate2D node (useless), use Rotator instead with value mul PI
Move amod to Transform type
Add 2 nodes : Xmirror & YMirror
