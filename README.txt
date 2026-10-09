DLC Client for Minecraft 1.21.4 (Fabric)

Keys (rebindable in Controls -> DLC Client):
  Right Shift or /dlc in chat - ClickGUI (LMB = toggle module, RMB = settings, drag sliders)
  R - AimAssist (works while holding LMB)
  G - TriggerBot
  H - AutoClicker (works while holding LMB, aimed at an entity)
  V - AutoSprint

Build (JDK 21):
  1. Go to https://fabricmc.net/develop/template/ , pick 1.21.4, generate a project.
  2. Easiest: copy only the src/ folder from this archive into the generated project.
     (Use the template's own build.gradle and gradle.properties - they have the correct versions.)
     Alternatively use this archive's build.gradle/gradle.properties as is.
  3. ./gradlew build
  4. Jar: build/libs/*.jar (not -sources) -> .minecraft/mods, with Fabric Loader and Fabric API for 1.21.4.

On joining a world you should see "[DLC] loaded" in chat and "DLC" at the top right.
If you don't, the mod isn't loaded: check the Minecraft version (1.21.4 only), Fabric Loader and Fabric API.

NO PC SETUP (build in the cloud):
  1. Create a free GitHub repo, upload ALL files from this folder (including the .github folder).
  2. Open the Actions tab -> wait for the "build" run to finish (about 2-3 min).
  3. Open the run -> Artifacts -> download "mod-jar" -> unzip -> drop the .jar into .minecraft/mods.
