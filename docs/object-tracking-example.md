#Object tracking
The Experimental Organization menu contains a `Scientific Object Tracking tool`. 

Searching filters allow selecting for scientfic objects such as plants, plots or organs or keywords.

 <div class="form-group">
  <label for="sel1">Parent type</label>
  <select class="form-control" id="sel1">
    <option>plant</option>
    <option>plot</option>
    <option>leaf</option>
    <option>ear inflorescence</option>
  </select>
</div> 

  <div class="form-group">
  <label for="usr">Keyword</label>
  <input type="text" class="form-control" id="usr" placeholder="e.g. arch">
</div>
<span class="btn btn-primary">Search</span> 

![](img/objecttrack1.png)

The filtered objects can be individually selected by clicking on left boxes and are automatically placed in a basket for further analyses. 

Selected objects can be visualised by clicking on the shopping car icon <a href="#" class="btn btn-warning">
          <span class="glyphicon glyphicon-shopping-cart"></span>     </a>

![](img/objecttrack2.png)

Once the objects are in the basket, different analyses ca be performed:

###Trait comparison
For instance different traits such as leaf area or plant height can be compared between selected objects
 <div class="form-group">
  <label for="sel1">Action</label>
  <select class="form-control" id="sel1">
    <option>Biovolume</option>
    <option>Leaf Area</option>
    <option>Plant height</option>
    <option>Thermal time</option>
  </select>
</div> 
<span class="btn btn-primary">Execute command</span> 

![](img/objecttrack3.png)

###Object inspection

The different icons on the right side of each selected object allow different actions:

- <p><a href="#"> <span class="glyphicon glyphicon-eye-open"></span> </a>: Allows browsing the object properties including annotations and events</p>

- <p><a href="#"> <span class="glyphicon glyphicon-cloud"></span> </a>: Allows visualisation of environmental conditions sensed by each object  </p>

- <p><a href="#"> <span class="glyphicon glyphicon-stats"></span> </a>: Allows visualisation of different time courses of traits </p>
<br>

For instance `biovolume` over time can be displayed together with the annotations and events (i.e. sowing, harvesting) that occured to a given plant:

![](img/objecttrack4.png)