# Tools menu

The Tools menu contains installation specific widgets and access to the Web Service API.

## URI Generator

URIs of new objects can be manually created using the URI generator. Upon declaration of a new URI, several fields are required such as `RDF label`, `RDF type`, `Date of creation` and `Comment`.

![urigenerator](img/urigenerator.png)

## Video Channels

For some installations having CCTVs or webcams, access is provided.

![cctv](img/cctv.png)

## Quick Response Code Generator

The tools menu contains a Quick response (QR) code generator. <button type="button" class="btn btn-default btn-sm"><span class="glyphicon glyphicon-qrcode"></span> Qrcode </button>

First, an experiment has to be chosen, and the list of plants or plots can be displayed.

<span class="btn btn-success">Visualise Plant Tags</span>

Plants or plots of a given experiment have a predefined Tag Pattern (e.g. `CAR_NUMBER/VARIETY/SEEDLOT/SCENARIO/REP/XY/EXPERIMENT`)

Tag patterns can be customised for each experiment. <span class="btn btn-warning">Change tag Pattern</span> 

QR codes can be customised using the different items available for each experiment. <span class="btn btn-primary">Configure QrCode Label</span>

For instance, information about the pot/plot number, the experiment, variety, scenario, seed lots, replicates and position of plants or plots can be displayed in QR codes:

![qrcode](img/qrcode.png)

*In the example QR code, 1080 and ARCH2017-03-30 stand for the pot number and experimnt name, respectivley*

Full details can be displayed in the following video:

<video width="320" height="240" controls> <source src="/vid/QRcodeGenerator.mp4" type='video/mp4'>
Your browser does not support the video tag.
</video>

## Web Service API

An link to the [Web Service API](webserviceAPI.md) is provided.