# Im-crashing-
Please Help!
Here is the Crash Report:




---- Minecraft Crash Report ----

WARNING: coremods are present:
  LoadingHook (Mekanism-1.10.2-9.2.0.294.jar)
  AppEngCore (appliedenergistics2-rv4-alpha-4.jar)
  EnderCorePlugin (EnderCore-1.10.2-0.4.1.60-beta.jar)
Contact their authors BEFORE contacting forge

// Who set us up the TNT?

Time: 11/23/16 10:36 PM
Description: Unexpected error

java.lang.NoClassDefFoundError: baubles/common/lib/PlayerHandler
	at vazkii.botania.common.core.handler.InternalMethodHandler.getBaublesInventory(InternalMethodHandler.java:186)
	at vazkii.botania.common.core.handler.InternalMethodHandler.getBaublesInventoryWrapped(InternalMethodHandler.java:191)
	at vazkii.botania.client.core.handler.BoundTileRenderer.onWorldRenderLast(BoundTileRenderer.java:68)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler_216_BoundTileRenderer_onWorldRenderLast_RenderWorldLastEvent.invoke(.dynamic)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:90)
	at net.minecraftforge.fml.common.eventhandler.EventBus.post(EventBus.java:185)
	at net.minecraftforge.client.ForgeHooksClient.dispatchRenderLast(ForgeHooksClient.java:166)
	at net.minecraft.client.renderer.EntityRenderer.func_175068_a(EntityRenderer.java:1400)
	at net.minecraft.client.renderer.EntityRenderer.func_78471_a(EntityRenderer.java:1229)
	at net.minecraft.client.renderer.EntityRenderer.func_181560_a(EntityRenderer.java:1038)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1076)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:371)
	at net.minecraft.client.main.Main.main(SourceFile:124)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:498)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)
Caused by: java.lang.ClassNotFoundException: baubles.common.lib.PlayerHandler
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:101)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:424)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:357)
	... 19 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Client thread
Stacktrace:
	at vazkii.botania.common.core.handler.InternalMethodHandler.getBaublesInventory(InternalMethodHandler.java:186)
	at vazkii.botania.common.core.handler.InternalMethodHandler.getBaublesInventoryWrapped(InternalMethodHandler.java:191)
	at vazkii.botania.client.core.handler.BoundTileRenderer.onWorldRenderLast(BoundTileRenderer.java:68)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler_216_BoundTileRenderer_onWorldRenderLast_RenderWorldLastEvent.invoke(.dynamic)
	at net.minecraftforge.fml.common.eventhandler.ASMEventHandler.invoke(ASMEventHandler.java:90)
	at net.minecraftforge.fml.common.eventhandler.EventBus.post(EventBus.java:185)
	at net.minecraftforge.client.ForgeHooksClient.dispatchRenderLast(ForgeHooksClient.java:166)
	at net.minecraft.client.renderer.EntityRenderer.func_175068_a(EntityRenderer.java:1400)
	at net.minecraft.client.renderer.EntityRenderer.func_78471_a(EntityRenderer.java:1229)

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityPlayerSP['achahdi'/619, l='MpServer', x=8.50, y=65.00, z=8.50]]
	Chunk stats: MultiplayerChunkCache: 0, 0
	Level seed: 0
	Level generator: ID 00 - default, ver 1. Features enabled: false
	Level generator options: 
	Level spawn location: World: (180,64,248), Chunk: (at 4,4,8 in 11,15; contains blocks 176,0,240 to 191,255,255), Region: (0,0; contains chunks 0,0 to 31,31, blocks 0,0,0 to 511,255,511)
	Level time: 0 game time, 0 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: survival (ID 0). Hardcore: false. Cheats: false
	Forced entities: 1 total; [EntityPlayerSP['achahdi'/619, l='MpServer', x=8.50, y=65.00, z=8.50]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:415)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2660)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:400)
	at net.minecraft.client.main.Main.main(SourceFile:124)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:498)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.10.2
	Operating System: Mac OS X (x86_64) version 10.11.6
	Java Version: 1.8.0_74, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 2748713512 bytes (2621 MB) / 4321705984 bytes (4121 MB) up to 26724532224 bytes (25486 MB)
	JVM Flags: 1 total; -Xmx28G
	IntCache: cache: 0, tcache: 0, allocated: 13, tallocated: 95
	FML: MCP 9.32 Powered by Forge 12.18.2.2147 20 mods loaded, 20 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCHIJAAAA	mcp{9.19} [Minecraft Coder Pack] (minecraft.jar) 
	UCHIJAAAA	FML{8.0.99.99} [Forge Mod Loader] (forge-1.10.2-12.18.2.2147.jar) 
	UCHIJAAAA	Forge{12.18.2.2147} [Minecraft Forge] (forge-1.10.2-12.18.2.2147.jar) 
	UCHIJAAAA	appliedenergistics2-core{rv4-alpha-4} [Applied Energistics 2 Core] (minecraft.jar) 
	UCHIJAAAA	mercurius_updater{1.0} [mercurius_updater] (MercuriusUpdater-1.10.2.jar) 
	UCHIJAAAA	appliedenergistics2{rv4-alpha-4} [Applied Energistics 2] (appliedenergistics2-rv4-alpha-4.jar) 
	UCHIJAAAA	Baubles{1.3.4} [Baubles] (Baubles-1.10.2-1.3.4.jar) 
	UCHIJAAAA	BiomesOPlenty{5.0.0.2080} [Biomes O' Plenty] (BiomesOPlenty-1.10.2-5.0.0.2080-universal.jar) 
	UCHIJAAAA	Botania{r1.8-320} [Botania] (Botania-unofficial.r1.8-320.jar) 
	UCHIJAAAA	endercore{1.10.2-0.4.1.60-beta} [EnderCore] (EnderCore-1.10.2-0.4.1.60-beta.jar) 
	UCHIJAAAA	mantle{1.10.2-1.1.1.194} [Mantle] (Mantle-1.10.2-1.1.1.jar) 
	UCHIJAAAA	tconstruct{1.10.2-2.5.3.jenkins387} [Tinkers' Construct] (TConstruct-1.10.2-2.5.3.jar) 
	UCHIJAAAA	immersiveengineering{0.10-44} [Immersive Engineering] (ImmersiveEngineering-0.10-44.jar) 
	UCHIJAAAA	JEI{3.13.3.373} [Just Enough Items] (jei_1.10.2-3.13.3.373.jar) 
	UCHIJAAAA	EnderIO{1.10.2-3.0.1.136_beta} [Ender IO] (EnderIO-1.10.2-3.0.1.136_beta.jar) 
	UCHIJAAAA	journeymap{1.10.2-5.2.4} [JourneyMap] (journeymap-1.10.2-5.2.4-unlimited.jar) 
	UCHIJAAAA	mcmultipart{1.2.0_74} [MCMultiPart] (MCMultiPart-experimental-1.2.0_74-universal.jar) 
	UCHIJAAAA	Mekanism{9.2.0} [Mekanism] (Mekanism-1.10.2-9.2.0.294.jar) 
	UCHIJAAAA	icse{1.1.0.0} [I Can See Everything] (Waila-Mod-1.10.2.jar) 
	UCHIJAAAA	wawla{2.3.0.194} [What Are We Looking At] (Waila-Mod-1.10.2.jar) 
	Loaded coremods (and transformers): 
LoadingHook (Mekanism-1.10.2-9.2.0.294.jar)
  
AppEngCore (appliedenergistics2-rv4-alpha-4.jar)
  appeng.transformer.asm.ASMIntegration
EnderCorePlugin (EnderCore-1.10.2-0.4.1.60-beta.jar)
  com.enderio.core.common.transform.EnderCoreTransformer
	GL info: ' Vendor: 'Intel Inc.' Version: '2.1 INTEL-10.14.73' Renderer: 'Intel Iris OpenGL Engine'
	AE2 Version: alpha rv4-alpha-4 for Forge 12.18.2.2104
	Pulsar/tconstruct loaded Pulses: 
		- TinkerCommons (Enabled/Forced)
		- TinkerWorld (Enabled/Not Forced)
		- TinkerTools (Enabled/Not Forced)
		- TinkerHarvestTools (Enabled/Forced)
		- TinkerMeleeWeapons (Enabled/Forced)
		- TinkerRangedWeapons (Enabled/Forced)
		- TinkerModifiers (Enabled/Forced)
		- TinkerSmeltery (Enabled/Not Forced)
		- TinkerGadgets (Enabled/Not Forced)
		- TinkerOredict (Enabled/Forced)
		- TinkerIntegration (Enabled/Forced)
		- TinkerFluids (Enabled/Forced)
		- TinkerMaterials (Enabled/Forced)
		- TinkerModelRegister (Enabled/Forced)

	EnderIO: No known problems detected.
	Detailed RF API diagnostics:
                  * RF API class 'EnergyStorage' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/EnergyStorage.class
                  * RF API class 'IEnergyConnection' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/IEnergyConnection.class
                  * RF API class 'IEnergyContainerItem' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/IEnergyContainerItem.class
                  * RF API class 'IEnergyHandler' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/IEnergyHandler.class
                  * RF API class 'IEnergyProvider' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/IEnergyProvider.class
                  * RF API class 'IEnergyReceiver' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/IEnergyReceiver.class
                  * RF API class 'IEnergyStorage' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/IEnergyStorage.class
                  * RF API class 'ItemEnergyContainer' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/ItemEnergyContainer.class
                  * RF API class 'TileEnergyHandler' is loaded from: jar:file:/Users/Chajdi/Library/Application%20Support/minecraft/mods/Mekanism-1.10.2-9.2.0.294.jar!/cofh/api/energy/TileEnergyHandler.class
	Detailed Tesla API diagnostics:
                  * Tesla API class 'Tesla' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.Tesla)
                  * Tesla API class 'TeslaCapabilities' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.capability.TeslaCapabilities)
                  * Tesla API class 'ITeslaConsumer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.ITeslaConsumer)
                  * Tesla API class 'ITeslaHolder' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.ITeslaHolder)
                  * Tesla API class 'ITeslaProducer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.ITeslaProducer)
                  * Tesla API class 'BaseTeslaContainer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.BaseTeslaContainer)
                  * Tesla API class 'BaseTeslaContainerProvider' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.BaseTeslaContainerProvider)
                  * Tesla API class 'InfiniteTeslaConsumer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaConsumer)
                  * Tesla API class 'InfiniteTeslaConsumerProvider' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaConsumerProvider)
                  * Tesla API class 'InfiniteTeslaProducer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaProducer)
                  * Tesla API class 'InfiniteTeslaProducerProvider' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaProducerProvider)

	AE2 Integration: IC2:OFF, RotaryCraft:OFF, RC:OFF, BuildCraftCore:OFF, BuildCraftTransport:OFF, BuildCraftBuilder:OFF, RF:OFF, RFItem:OFF, MFR:OFF, DSU:OFF, FZ:OFF, FMP:OFF, RB:OFF, CLApi:OFF, Waila:OFF, InvTweaks:OFF, JEI:ON, CraftGuide:OFF, Mekanism:OFF, ImmibisMicroblocks:OFF, BetterStorage:OFF, OpenComputers:OFF
	Launched Version: 1.10.2-forge1.10.2-12.18.2.2147
	LWJGL: 2.9.2
	OpenGL: Intel Iris OpenGL Engine GL version 2.1 INTEL-10.14.73, Intel Inc.
	GL Caps: Using GL 1.3 multitexturing.
Using GL 1.3 texture combiners.
Using framebuffer objects because ARB_framebuffer_object is supported and separate blending is supported.
Shaders are available because OpenGL 2.1 is supported.
VBOs are available because OpenGL 1.5 is supported.

	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: 
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	CPU: 4x Intel(R) Core(TM) i5-4258U CPU @ 2.40GHz
