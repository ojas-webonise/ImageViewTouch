ImageViewTouch
==============

Pinch / dubble tap zoom-in, zoom-out for image view and at the same time handling the swipe events on the same ImageView 


How to add library :

- This can be either 
     used as a library project (project properties->Android->add Library) 
  or 
     add ImageViewTouch.jar file from ImageViewTouch->bin to libs folder in your project
     
     
How to use :

   You can use ImageViewTouch in your project as below,
   
   
   First create a widget in your layout
   
    <com.imagezoom.ImageViewTouch 
    android:id="@+id/imageViewTouch"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
   
   
   
   Creating instance of ImageViewTouch in your class
   ImageViewTouch mImageView = (ImageViewTouch) findViewById(R.id.imageViewTouch);
   
   Setting display type for how the image should adjust 
   mImageView.setDisplayType( DisplayType.FIT_IF_BIGGER );
   
	mImageView.setListener(new SwipeListener() {
	
	@Override
	public void onSwipeRightToLeft() {
	  //Perform the action required
	}
					
	@Override
	public void onSwipeLeftToRight() {
	  //Perform the action required
	}
	}				

