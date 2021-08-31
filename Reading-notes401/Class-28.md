# Create dynamic lists with RecyclerView  

- RecyclerView makes it easy to efficiently display large sets of data. You supply the data and define how each item looks, and the RecyclerView library dynamically creates the elements when they're needed.

- RecyclerView recycles those individual elements. When an item scrolls off the screen, RecyclerView doesn't destroy its view. Instead, RecyclerView reuses the view for new items that have scrolled onscreen. This reuse vastly improves performance, improving your app's responsiveness and reducing power consumption.

- Besides being the name of the class, RecyclerView is also the name of the library. In this page, RecyclerView in code font always means the class in the RecyclerView library.

## in conclusion : 
## waht is recyclerView ?
it provides a fixed size window so that we can load a large data.

 ## Key Classes 
 it's a multiple classes that are used to build a dynamic list. 

 * RecyclerView is the ViewGroup that contains the views.notice that it's a view itself so we can add it to the layout.

 * View holder object : each element in the list. once it's created will be binded to the RecyclerView (RecyclerView.ViewHolder.) using RecyclerView.Adapter

 *  layout manager to arrange the individual elements in the list.

 ## Implementing the RecyclerView 
  
  * we should add the RecyclerView AndroidX library to gradle.build 

  * create a model class to be as a data source.
  * add RecyclerView to activity to display items. 

  * create a layout XML to view the item.

