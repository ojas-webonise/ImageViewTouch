ImageViewTouch
==============

Pinch / double tap zoom-in, zoom-out for image view and at the same time handling the swipe events on the same ImageView 


#How to add library :

- You can either 
     use this as a library project (project properties->Android->add Library) 
  or 
     add ImageViewTouch.jar file from ImageViewTouch->bin to libs folder in your project
     
     
#How to use :

   You can use ImageViewTouch in your project as follows.
   
   
   First create a widget in your layout
   
    <com.imagezoom.ImageViewTouch 
    android:id="@+id/imageViewTouch"
    android:layout_width="match_parent"
    android:layout_height="match_parent" />
   
   
   
   Then find it from your code
   
   	ImageViewTouch mImageView = (ImageViewTouch) findViewById(R.id.imageViewTouch);
   
   Set how the image should adjusted
   
   	mImageView.setDisplayType( DisplayType.FIT_IF_BIGGER );
   	
   Setting listener for swipe action on image view
   
	mImageView.setListener(new SwipeListener() {
	
	    @Override
	    public void onSwipeRightToLeft() {
	        //Perform the required action
	    }
					
	    @Override
	    public void onSwipeLeftToRight() {
	        //Perform the required action
	    }
	}				

