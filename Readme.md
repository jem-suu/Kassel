# Kassel Kerbs for OMSI 2

Hi, and thanks for downloading the Kassel Kerb set for OMSI 2. Originally for a map project I started (then abandoned), I decided to make these kerbs available for all devs to use.

I recommend to use the [UKDT DevKit Pathways pack](https://fellowsfilm.com/downloads/ukdt-devkit-vol-1-pathways.1578/) alongside these kerbs, as these were originally made to fit along with them and they contain pavement splines that can help with filling gaps behind the kerbs themselves.

# Including with your map

Please note, **This should not be a dependency for your map.**

It is recommended to bundle these with your ScenryObjects/Splines library for your map so that installation is much easier.

To bundle with your map, copy the contents of the `SceneryObjects` folder to your map's Sceneryobjects Library, commonly
```X:\OMSI 2\SceneryObjects\<your_map_name>```.

The same should be done with the contents of the `Splines` folder, also
```X:\OMSI 2\Splines\<your_map_name>```.

# Usage

The pack contains two sizes of Kerbs: `160`mm and `180`mm. Each contains four objects:

- Start Piece
- End Piece
- Internal Corner Piece
- External Corner Piece

and a spline for each kerb height.

The kerbs can be placed atop the existing kerbline if the map is using the **UKDT Devkit: Pathways**, otherwise the pavement will have to be adjusted to match the height. Both the splines and the objects have been built so that the centres of each are in line with the outer edge of the kerb.

For the pavement spline that would sit behind the kerb, I recommend using the 1m Pathway from the UKDT Pathways pack, and make a series of splines following this formula.

(`x` in this context is the length of the main kerb spline, `y` means the radius of the kerb spline)

### 160mm

Spline | 1 | 2 | 3
- | - | - | -
**Length** | 1m | `x` m | 1m 
**Radius** | N/A | (`y`-0.4) m | N/A 
**Gradient** | <p>Start: 3%</p><p>End: 3%</p> | <p>Start: 0%</p><p>End: 0%</p> | <p>Start: -3%</p><p>End: -3%</p> 
**Cant** | <p>Start: 0%</p><p>End: -6%</p> | <p>Start: -6%</p><p>End: -6%</p> | <p>Start: -6%</p><p>End: 0%</p> 

### 180mm

Spline | 1 | 2 | 4
- | - | - | -
**Length** | 1m | `x` m | 1m 
**Radius** | N/A | (`y`-0.8) m | N/A 
**Gradient** | <p>Start: 4%</p><p>End: 4%</p> | <p>Start: 0%</p><p>End: 0%</p> | <p>Start: -4%</p><p>End: -4%</p> 
**Cant** | <p>Start: 0%</p><p>End: -8%</p> | <p>Start: -8%</p><p>End: -8%</p> | <p>Start: -8%</p><p>End: 0%</p> 

# Copyrights

`work on this bit, you're releasing it on git as well`