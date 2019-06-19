<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Weasly clock</a>
<ul>
<li><a href="#sec-1-1">1.1. Design Goals/Plans</a></li>
<li><a href="#sec-1-2">1.2. Related Projects for Inspiration</a></li>
<li><a href="#sec-1-3">1.3. Notes on parts</a></li>
</ul>
</li>
<li><a href="#sec-2">2. Shoppting list</a>
<ul>
<li><a href="#sec-2-1">2.1. Shopping list from Servo City servocity.com</a></li>
<li><a href="#sec-2-2">2.2. Shopping list from Hobbylinc </a></li>
<li><a href="#sec-2-3">2.3. Notes on parts</a></li>
</ul>
</li>
</ul>
</div>
</div>



# Weasly clock<a id="sec-1" name="sec-1"></a>

Build a working physical Weasley Clock from Harry Potter. 

## Design Goals/Plans<a id="sec-1-1" name="sec-1-1"></a>

-   use a Raspberry Pi to control clock via servos and servo hat
-   physical hands, each moving independently
-   four (4) physical hands, one for each family member
-   build my own clockwork
-   program in python
-   use live GPS data of family members
-   GPS updates from one or more of: iCloud, Owntracks, life360, local MQTT, and/or local network device scanning

## Related Projects for Inspiration<a id="sec-1-2" name="sec-1-2"></a>

-   <https://www.instructables.com/id/Build-Your-Own-Weasley-Location-Clock/>
-   <https://printableprops.jimdo.com/en/harry-potter/weasley-clock/>
-   <https://www.instagram.com/printableprops/>
-   <https://fourierinformationsir.wordpress.com/2015/11/09/weasley-clock-update/>
-   <https://twitter.com/wbtourlondon/status/765398939910627328?lang=mr>

## Notes on parts<a id="sec-1-3" name="sec-1-3"></a>

-   Servo control
    servo hat: <https://www.adafruit.com/product/2327>
    Servo: <https://www.servocity.com/hs-785hb-servo>
    -   <https://www.servocity.com/32p-24t-c1-spline-servo-mount-gears-metal>
        32P, 24T C1 Spline Servo Mount Gears (Metal)
        NOTE: These don't clear the servo body, need a smaller servo? or stagger the
        gears.
    -   hubs for servo gears: <https://www.servocity.com/standard-hub-horns>
    -   <https://www.servocity.com/32-pitch-50-bore-aluminum-hub-gears>
           1/2" Bore 32 Pitch Aluminum Hub Gears
    -   mounting nuts for al hub gears.

# Shoppting list<a id="sec-2" name="sec-2"></a>

## Shopping list from Servo City servocity.com<a id="sec-2-1" name="sec-2-1"></a>

-   4 HS-785HB SERVO   SKU: 33785S
-   3 32T, 0.250" (1/4) Bore 32P Shaft Mount Pinion Gear SKU: 615254
-   1 32P, 32 Tooth, 24T C1 Spline Servo Mount Gear (Metal)
-   3 C1 SPLINE SERVO TO 1/4" SHAFT COUPLER (SET SCREW) SKU: 525134
-   3 0.250" (1/4") X 2.50" (2-1/2") STAINLESS STEEL D-SHAFTING SKU: 634074
-   4 32 Pitch, 64 Tooth (.50" Bore) Aluminum Hub Gear        615194
-   6mm (0.770") Clamping Hub   545616
-   5mm (0.770") Clamping Hub        545612
-   4MM (0.770") CLAMPING HUB SKU: 545608
-   3MM (0.770") CLAMPING HUB SKU: 545604

## Shopping list from Hobbylinc <https://www.hobbylinc.com/htm/k+s/k+s9821.htm><a id="sec-2-2" name="sec-2-2"></a>

-   NOTE: checked items are a good set for a 4 hand clock. Theoretically

possible to create a 6 hand clock with all of the sizes. However,
servocity doesn't sell clamping hubs for size 2mm and 7mm.
-   parts:
    -   [ ] 2mm x 300mm Round Brass Tube .45mm Wall (4) k+s9820 Item # K+S9820
    -   [X] 3mm x 300mm Round Brass Tube .45mm Wall (4) k+s9821 Item # K+S9821
    -   [X] 4mm x 300mm Round Brass Tube .45mm Wall (3) k+s9822 Item # K+S9822
    -   [X] 5mm x 300mm Round Brass Tube .45mm Wall (3) k+s9823 Item # K+S9823
    -   [X] 6mm x 300mm Round Brass Tube .45mm Wall (2) k+s9824 Item # K+S9824
    -   [ ] 7mm x 300mm Round Brass Tube .45mm Wall (2) k+s9825 Item # K+S9825

## Notes on parts<a id="sec-2-3" name="sec-2-3"></a>

-   <https://www.servocity.com/32p-24t-c1-spline-servo-mount-gears-metal>
    NOTE: The 32 tooth gears don't fully clear the servo body. This
    means that to use more than one servo, we need to use a shaft so
    that central 64 tooth gears don't hit/interfere with the servos.
-   Using 64 tooth gears mounted to the brass tubes. This gives a clean
    1:2 ration from the servos.
-   The HS-785HB Servos have a claimed 8 full rotations. I only need 2
    full rotations to get the full range of motion of the clock
    hands. Having more than 360 degrees of motion allows for a little
    **flair** when positioning the hands. I'm going to use just 6 full
    rotations of the servo (so 3 full rotations of the hands) to avoid
    using the extremes of the PWM signals to the servos.
