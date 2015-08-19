AstroWS
=======

AstroWS is a set of web services about astrology.

Dependancies
------------

    sudo pip install pyswisseph 4Suite-XML

Services
--------

### chartinfo.py

#### Description

Returns houses, bodies positions, aspects and conjunctions for a given place and datetime.

#### Arguments

#### Exemple call

<http://astro.kivutar.me/chartinfo.py?name=Anthony%20Tran&city=New%20York%20City&lat=40.7127&lon=-74.0059&year=1989&month=4&day=26&time=16.8&hsys=E&display=0,1,2,3,4,5,6,7,8,9,10,12,23>

### transform.py

#### Description

XSLT processor, used to generate SVG natal chart from chartinfo.py output.

#### Exemple call

<http://astro.kivutar.me/transform.py?xml=http%3A%2F%2Fastro.kivutar.me%2Fchartinfo.py%3Fname%3DAnthony%2520Tran%26city%3DNew%2520York%26lat%3D40.71427%26lon%3D-74.00597%26year%3D1989%26month%3D04%26day%3D26%26time%3D16.8%26hsys%3DE%26display%3D0%2C1%2C2%2C3%2C4%2C5%2C6%2C7%2C8%2C9%2C10%2C12%2C23&xsl=wheel.xsl>

### rasterize.py

#### Description

SVG to PNG converter.

#### Exemple call

<http://astro.kivutar.me/rasterize.py?svg=http://www.croczilla.com/svg/samples/lion/lion.svg>

Frontend
--------

We provide an xHTML form at <http://astro.kivutar.me/gui/form.html> as frontend to AstroWS.
