# Tools menu

The Tools menu contains installation specific widgets and access to the Web Service API.

##URI Generator

##Video Channels
For some installations having CCTVs or webcams, access is provided. 

## Quick Response Code Generator  

The tools menu contains a Quick response (QR) code generator. <button type="button" class="btn btn-default btn-sm">
          <span class="glyphicon glyphicon-qrcode"></span> Qrcode 
        </button>
      

First, an experiment has to be chosen, and the list of plants or plots can be displayed.

<span class="btn btn-success">Visualise Plant Tags</span> 

Plants or plots of a given experiment have a predefined Tag Pattern (e.g. `CAR_NUMBER/VARIETY/SEEDLOT/SCENARIO/REP/XY/EXPERIMENT`)

Tag patterns can be customised for each experiment. <span class="btn btn-warning">Change tag Pattern</span> 

QR codes can be customised using the different items available for each experiment. <span class="btn btn-primary">Configure QrCode Label</span>

For instance, information about the different treatments, seed lots, replicates and position of plants or plots can be displayed. And QR codes generated for the whole experiment. 

<video width="320" height="240" controls>
 <source src="/vid/QRcodeGenerator.mp4" type='video/mp4'>
Your browser does not support the video tag.
</video> 

##Web Service API

The web service API enables interoperability and data exchange with other applications and systems. It can be accessed via a user account and a limited encrypted token. The web service  is based on RESTFul (Representational state transfer) developed using Swagger framework [https://swagger.io/](https://swagger.io/) and all services are available by using URIs. It is developed in Java with Jersey implementation of JAX-RS (Java API for RESTful Web Services) standard. It implements the [Breeding API (BrAPI)](http://www.brapi.org/), which specifies a standard interface for plant phenotype databases to serve data to crop breeding applications. Web service outputs use the data-interchange format JSON (JavaScript Object Notation). The Web services and access are described at [http://web.supagro.inra.fr/phis/phenomeapi/api-docs/](http://web.supagro.inra.fr/phis/phenomeapi/api-docs/) and are available to authorized client programs. 
