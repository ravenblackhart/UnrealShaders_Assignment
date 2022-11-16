# UnrealShaders_Assignment
FGGP21 Shaders Assignment

All shaders and effects are present in the following maps (Content > Maps) 
1. 0_Default - Using base from Asset pack with shaders applied for a more "realistic" application 
2. ThirdPersonMap - Standalone Applications to defualt Unreal ThirdPerson starting map to allow effects to be more visible individually. 

##Shaders Included 
These Materials can be found in Content > Materials
1. M_Bubble_Static - Bubble Material
2. M_Bubble_Floating - Floating Variation of Bubble material that warps over coordinates
3. M_SingleLayerWater - Water Material to simulate movement and refraction, taking nearby / overlap surfaces into consideration 
4. MI_CauldronLiquid - Instance Variation of M_SingleLayerWater to simulate boiling liquid
5. M_ToonShader - Post-Processing Shader to Outline Objects 

##Some of the Above have been used in the following Components : 
In Content > VFX , 
1. N_CauldronBubbles - M_Bubble_Static + M_Bubble_Floating in 2 Emitters 
2. N_Water - M_Bubble_Floating in 1 emitter 
3. BP_Outline_PPV - M_ToonShader 

In Content > LevelPrototyping > Custom, 
1. Cauldron - Includes MI_CauldronLiquid + N_CauldronBubbles
