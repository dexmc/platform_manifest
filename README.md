#Initialize the source
repo init -u https://github.com/SimpleAOSP-Lollipop/platform_manifest.git -b L

#Sync the source
repo sync -jx -f (x being however many cpu jobs)

#Setup build environment
. build/envsetup.sh

#Choose supported device to build
lunch simpleaosp_flo-user, lunch simpleaosp_hammerhead-user, lunch simpleaosp_mako-user or lunch simpleaosp_shamu-user

#Build it
mka otapackage

#Credits
Google for AOSP, Rascarlo and Rastakat for a lot for commits, DariosF and Purity ROM, AOSPAL, AOSPA, CM, DirtyUnicorns, SaberMod, LiquidSmooth
,AOKP, SlimRoms, Project D.I.S.C.O. team, PartimusPrime for bootanimations, OmniRom, Others that we may missed
