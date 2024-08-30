Using Visual Format Language, with a single line of code, you can specify multiple constraints in either the horizontal or vertical direction.

Available Symbols in VFL:
| superview
- standard spacing (usually 8 points; value can be changed if it is the spacing to the edge of a superview)
== equal widths
-10- non standard spacing (10 points)
<= less than or equal to
>= greater than or equal to
@250 priority of the constraint, can have any value between 0 and 1000.
Visual Format Syntax:-
H: Indicates horizontal orientation.
V: Indicates vertical orientation.
If you’re not mentioning H:/V:, Auto Layout defaults to horizontal orientation.
Spacing — it defines space between the two views. If you provided space value explicitly, Autolayout takes that value to define space between views else default spacing 8 will be added.
View with default spacing can be represented as: [view1]-[view2]
View with custom spacing can be represented as: [view1]-10-[view2]
View without spacing can be represented as: [view1][view2]
[View] — View that laying out required
Width Constraint: used for adding width to view. You need to provide width of views into horizontal constraints.
Width of view with greater than or equal to constant can be represented as: [View(>=constant)] .e.g View width ≥50 is represented as: [View(>=50)]
Width of view with less than or equal to constant can be represented as: [View(<=constant)]. e.g: View width ≥50 is represented as: [View(<=50)]
Width of view equal to constant can be represented as: [View(constant)]. e.g: View width = 50 is represented as: [View(50)]
Height Constraint: used for adding height to view. You need to provide Height of views into vertical constraints.
Height of view with greater than or equal to constant can be represented as: V:|[View(>=constant)] .e.g View height ≥50 is represented as: V:|[View(>=50)]
Connection to Superview(|) : Used for connecting view with superview
Connecting view to superview with default spacing as: |-[view]-|
Connecting view to superview with custom spacing as: |-constant-[view]-constant-|. e.g: |-50-[button]-50-|
Priority : Can be set as [view(widthValue@priorityvalue)]. e.g: [view(50@250)]
Equal Widths : equal width of two views can be represented as [View1(==View2)]
Multiple Predicates: multiple predicates of view can be represented as [view1(>=constant,<=constant)]. e.g: [view1(>=70,<=100)]




