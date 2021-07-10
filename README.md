# mindustry-mod-abcde-whiteplanet
just a planet based on Serpulo size: 4 

code display: 

const abcde = new JavaAdapter(Planet, {}, "abcde", Planets.sun, 4, 1); 
// the first number represents its size thus its number of locations. putting this number to 5 or greater will result the game crash
abcde.generator = new SerpuloPlanetGenerator(); // generator built in the original game
abcde.mesh = new HexMesh(abcde, 5); // for hud up oh hover decoretion . Not imortant
  abcde.orbitRadius = 100; // distance from the sun
    abcde.orbitTime = 1500; 
    abcde.rotateTime = 30;
    abcde.bloom = false;
    abcde.accessible = true; // needed
    abcde.startSector = 1; 
    abcde.hasAtmosphere = false;
    abcde.atmosphereColor = Color.valueOf("63353cFF");
    abcde.atmosphereRadIn = 0.0;
    abcde.atmosphereRadOut = 0.0;
    abcde.alwaysUnlocked = true; // needed to access the planet
    abcde.localizedName = "abcde"; // the name of the planet

var h = new SectorPreset("a1", abcde, 1); 
// currenlty does not work for this stage in terms of difficulty but needed to proceed to the rest of the planet.  
h.difficulty = 1; 
h.alwaysUnlocked = true;
h.captureWave = 12; 
h.localisedName = "1a";

Now try this yourself. Maybe a tiny Serpulo. 
