I left a lot of settings that I believe to be entirely or almost completely user preference commented out.
Hopefully this file can help you find what you may want/need to change.

NoTutorial.cfg					
  Disables tutorial prompts/dialog
  
SteamController.cfg			
  Settings for Steam Controllers
  Most of this config is commented out.
  
HUDNotifications.cfg			
  Contracts, Vote UI, Achievement tracking, Killstreaks, Chat
  Most of this config is commented out.

HUDGeneral.cfg					
  Most HUD settings can be found here. Some of this is actually relevant to performance

UserPreferences.cfg			
  User Preferences including hitsounds, damage numbers, FOV, 
  viewmodels, crosshair, closed captions, ingame demo settings, etc.
  Most of this config is commented out.
  
NetSettings.cfg				
  You'll find most/all net settings here including match making settings
  I encourage people to setup class configs like such
  scout.cfg
  soldier.cfg
  pyro.cfg
  demoman.cfg
  heavyweapons.cfg
  engineer.cfg
  medic.cfg
  sniper.cfg
  spy.cfg
  And put in their preffered "cl_interp" on a per class basis. 
  Generally speaking cl_interp should be as low as possible for projectile/particle based classes
  Pyro, Soldier, Demoman, Medic
  cl_interp 0.0152
  While hitscan classes should give enough headroom for a dropped or delayed server update to the client.
  Scout, Heavy, Engineer, Sniper, Spy
  cl_interp 0.0304
  If you don't want to bother with setting up class configs I set the config to be cl_interp 0.0304 which
  should still be a improvement over default TF2 regardless of weapon type for users with stable internet 
  connections. If you don't have a stable internet connection you can try higher values in multiples of 
  0.0152 like 0.0456 and 0.0608.
  Technically cl_interp_ratio would be a better way of setting up interp in an appropriate manner, but a lot
  of league server configs and sometimes community servers force cl_interp_ratio 1, and is set as such in 
  this config.
  
Sound.cfg						
  Most/All sound settings can be found here including volume.
  
gfxc.cfg						
  The main part of the performance config
  
  For other performance config users
  If you're curious why your game suddenly looks really different or why you shader options are "High" ingame
  it's because mat_reducefillrate is now set to 0. In DX9 this performs a fair amount better than
  mat_reducefillrate 1. In DX8 the affect on FPS is negligible/nonexistant assuming you have a decent GPU.
  
TransparentViewmodels.cfg	
  If you use transparentviewmodels go to "autoexec.cfg" and remove this // from in front of the 
  "exec TransparentViewmodels.cfg" line.