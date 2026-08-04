Want to be a feline on VRChat? I've made a collection for you to use or to personalize to your heart's content!

PLEASE NOTE: You'll need a basic working knowledge of Unity and the VRChat 3.0 SDK to upload these avatars as well as Substance Painter if you wish to retexture them. Unfortunately I can't help with general avatar setup questions, but the official VRChat SDK guide at https://docs.vrchat.com/docs/setting-up-the-sdk is a great place to start!

Features:
   VRChat Avatar 3.0 Model
   Fullbody Tracking compatible
   14 blendshape expressions
   Full blendshape visemes
   VIVE compatible eye and face tracking visemes
   Blender file for Avatar and all accessories
   Substance Painter projects for avatar and all accessories
   10 base model configurations:
      Lynx Male/Female
      Sabertooth Male/Female
      Cheetah Male/Female
      Snow Leopard Male/Female
      Lion/Lioness
   Adjustable body proportions via blendshapes:
      Hips
      Waist
      Calves
      Feet
      Thighs
      Back
      Arms
      Hands
      Neck
      Head
      Breasts
      Claws
      Saber teeth
   Audio features:
      Selectable purr
      Selectable scratch
   Adjustable ear type via blendshapes:
      Big cat (round)
      House cat
      Lynx (tufted)
   Adjustable polygon fur via blendshapes:
      Check fluff
      Ear fluff
      Chest fluff
      Leg fluff
      Butt fluff
      Crotch fluff
      Tail fluff
      Lynx fluff
   Multiple tail types
      Sabertooth nub tail
      Lynx nub tail
      Lion tail
      Tiger/Cheetah/Housecat tail
   Multiple Accessories
      Golden arm and leg cuffs
      Bow tie and tux cuffs
      Right and left ear rings
      Nose ring
      Sunglasses
      Harness
   
Requirements:
   - The latest VRChat Avatar 3.0 SDK unity package: https://vrchat.com/home/download
      
Installation:
   - Import the latest VRChat Avatar 3.0 SDK unity package. (https://vrchat.com/home/download). 
   - Import the Feline avatar unity package.
   - Open Feline_Scene under Assets/Feline/Scenes/
   - Select your avatar and upload! If you're new to Unity and the VRChat SDK and you'd like to have a go at editing your avatar, I'd highly recommend Sippbox's Youtube channel and his very helpful Avatar 3.0 tutorial series here: https://www.youtube.com/channel/UCsQ86hFQ6wxX_CsWMp8DJVw
    
Performance Optimized Avatars:
   - There are two sets of avatars included in the unity project: Full-Featured and Performance Optimized. The performance optimized avatars are disabled by default, but can be enabled in the Unity scene if you desire a medium performance rating. They have the ear and nose rings, grabbable sunglasses, and most physbones removed.
   
Notes on Customizing Avatars:
   - Each Avatar prefab in the included Unity scene contains multiple meshes for items such as alternate tails, a mane, and accessories. In order to keep the Avatar performance rating as high as possible, unused meshes are disabled and their skinned mesh renderers removed. If you would like to enable one of these items for a custom avatar, enable it by taking the following steps:
      - Click on the avatar you want to modify in the scene hierarchy window and open its hierarchy
      - Select the Tail/Mane/Accessory that you'd like to enable
      - In the inspector window, click the checkbox in the top left corner to enable the item, then click on the gear icon next to the component labeled "Skinned Mesh Renderer (Removed)" and choose Removed Component > Revert.
   - Conversely, if you want to disable an item on an avatar simply select the item in the Avatar's hierarchy, click on the gear icon next to that item's skinned mesh renderer in the Inspector window, and choose "Remove Component".
   
Notes Source Files:
   - The FBX model file used for the avatar prefab is located at
      Assets/Feline/Source Files/Blender/Feline_Base.fbx
   - The Blender source file used to generate the FBX is located at
      Assets/Feline/Source Files/Blender/Feline_Base.blend
   - The Substance painter projects for generating the avatar textures are located at
      Assets/Feline/Source Files/Substance_Painter/

Notes Substance Painter Projects:
   - There is a single substance painter file, Base.spp, for all of the avatar variants. Textures for each species are separated into folders inside the Substance project; simply show the folder for the species you want to edit and hide the rest.
   - Notes on editing the substance painter project:
      - After opening the substance project, disable the texture-set labeled "!DISABLE ME!" along with any other texture-sets you're not interested in editing.
      - For each species, there is a folder under "Fur" marked "Emissive Markings". You can edit the layers in this folder to paint markings on your character which will automatically be filled with a color gradient. Here's how to do so:
         - Open the "Emissive Markings" folder and select the "Stripes Paint" or "Markings Paint" fill layer.
         - Set the fill color to whatever initial color you want your character's markings to be.
         - Select the layer mask and remove the existing markings using the eraser or polygon fill tool. DO NOT use "clear mask" or "remove mask" as it will destroy the mask anchor used to create the color fill!
         - If you want your character's main (Albedo Transparency) texture to include color-filled markings, enable the "[Auto] Center Fill" layer.
         - If you want your character's emissive texture to include color-filled emissive markings, enable the "[Auto] Emissive" layer. Emissive markings will be controllable via the emission slider in the in-game Avatar V3.0 menu.
   - I have made a small edit to fix the UV map in the right eye socket since the substance painter project was created. This shouldn't be an issue since the eye sockets are behind the eyes and intended to be flat black, but you can enable the "Final UV Overlay" layer if you need to make any detailed changes in that area. Just make sure to disable again before exporting!
   - The easiest way to export your new textures is to overwrite the texures of one of the base models. Click on File > Export Textures, select the Body, Eyes, Cuffs, and Mane, depending on which materials you've changed, and set the output directory to "Assets/Feline/Textures/[Species]" depending on your chosen avatar. 
   - Several accessories also have their own substance painter files; their textures have been exported to the Assets/Feline/Textures/Common/ folder.

If you have any questions about these avatars please contact me at
   Twitter : http://twitter.com/revitfur
   Email   : avatars@sabermade.com

Changelog : V1.1 2020/12/26
   - Snep (Male/Female Full/Optimized)
      - Reset default mood_idlesmile blendshape to 0
      - Fixed bad reference to head tuft material
   - Base.spp
      - Fixed some texture issues on paw pads
      - Small clean-ups of the fur underlay
 
Changelog : V1.2 2021/01/02
   - Updated readme with correct link to Dynamic Bone script
   - Tweaks to eyes-closed blendshape to prevent eye clipping through eyelids between 20-37%
   - Tweaks to shoulder armature to prevent neck clipping when arms are raised
   - Tweaks to leg armature to improve standing pose
   - Fixed lion tail bending abnormally while sitting with FBT
   - Fixed inner eye socket vertices driven by fur blendshapes
   - Fixed left thumb extents

Changelog : V1.21 2021/01/07
   - Fixed broken whiskers on Lynx Male and Lynx Male (Opt) avatars
   
Changelog : V1.30 2021/04/29
   - Updated compatibility for VRChat SDK3 2021.03.22.18.27
   - Converted many avatar parameters to boolean in order to free up extra parameter slots
   - Added several alternative rest (silence) visime blendshapes - vrc.c_sil_alt(1-3)
   - Added nose shape blendshape
   - Added 42 facial-tracking blendshapes. These blendshapes are designed to be compatible with applications using HTC vive eye and face tracking hardware. These blendshapes all have names beginning with ft.*. Don't have face tracking? You could also mix-and-match them to make your own expression animations!
   - Added harness and collar accessory in both male and female variants, including Substance Painter source file for textures.
   - Set body-neck_shrink blendshape to 50% on most avatars.
   - Renamed the chest mane bone on the armature to allow for easier import into Neos
   
Changelog : V1.40 2022/06/03
   - Updated all avatars from dynamic bone to physbones
   - Added armature bones for toes and enabled physbones for full-body users
   - Added armature bones for harness and enabed grabbable physbones
   - Added 'booty' blendshape and slider
   - Updated weight painting on harness
   - Removed redundant hand colliders
   - Added floor collider for feet and tail
   - Added placeholder muzzle and feet colliders - connect them up as you like
   - Updated Poiyomi shader to V7.3.046
   - Enabled Audio Link on avatars with emissive maps
   
Changelog : V1.41 2024/01/21
   - Fixed "Load in Background" error for audio clips when project opened in newer versions of VRC SDK.
