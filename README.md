## MMScalableVectorView
Turns static PaintCode or Qwarkee code into a UIView that honors its contentMode property.
<table>
<tr>
<td><div align="center"><b>Before</b></div></td>
<td><div align="center"><b>After</b></div></td>
</tr>
<tr>
<td><img src="http://michaelmaxwell.info/wordpress/wp-content/uploads/2013/12/normalVector.png" width="270px"></td>
<td><img src="http://michaelmaxwell.info/wordpress/wp-content/uploads/2013/12/scaledVector.png" width="270px"></td>
</tr>
</table>


## Installation
##### CocoaPods

##### Manually
Just import MMScalableVectorView.m & .h into your project directly.

## Usage

1. Create a new class to represent the graphic, and make sure it inherits from MMScalableVectorView.
2. Implement the following methods:
	1. Paste the Qwarkee/PaintCode drawing code into `drawInCurrentContext`
	2. Implement `originalSize` to return a `CGSize` structure for the native size of the vector graphic.
3. Use the newly created class as a normal UIView, setting the `contentMode` property as desired before the view is drawn. This can be done in Interface Builder or programatically.


## Future Improvements
  
  
UIView category with a block-based initializer for one-stop creation of vector-backed UIViews.
Improving drawing when UIView’s transform property is used (?)
Unit tests!