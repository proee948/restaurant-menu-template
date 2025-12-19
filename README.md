# RESTAURANT-MENU-TEMPLATE
is designed to be an easy to modify,implement and copy paste template for QR CODE restaurant menu systems.

# FEATURES
1. simple and user friendly interface.
2. locked aspect ratio (no pinch zoom) which gives a professional vibe.
3. multiple language support (croatian,english,german,italian,philipino).
4. modular currency conversion algorithm (BAM to EUR default).
5. DISH 3D VIEWER (more on this below).
6. usual optimization techniques like lazy loading and atlas pictures.

# DISH 3D VIEWER
dish 3D viewer is an addition to this menu meaning it is completely optional, if needed it can be completely removed.

the viewer uses Javascript to load an image inside a popup window, the window contains the loaded image(meant to be an texture atlas) and a user friendly smooth slider for sliding the picture along 5-DIRECTIONAL VIEW(can be more directions as long as ASPECT RATIO limitation is met).

the viewer, by default expects a TEXTURE ATLAS. meaning one picture that contains (n) amount of smaller pictures, which JS then processes and loads according to their X and Y coordinates.

the default set by myself is a HORIZONTAL TEXTURE ATLAS(VERTICAL NOT SUPPORTED!!!!! as of yet) containing no more than (n) pictures whose combined aspect ratio equals 2048 x 2048 px... this aspect ratio however shall not be exceeded due to issues of android/IOS devices, if this safety ceiling were however to be exceeded, certain loading errors will occur, so its best to leave it be and work within its constraints. ||||to be clear atlas.png or any other atlas SHALL NOT exceed 2048 x 2048! for compatibility reasons||||

even though the viewer is called 3D it is by no means a 3D graphical scan of a dish, it simply uses pictures and allows sliding across them rapidly and thus gives an illusion of having a real object infront of you in three dimensions. having an actual 3D rendered system for each dish would be incredibly inneficient,hard to do and would look like dogshit.

the atlas system expects a napoli_atlas.png like structure of a picture, meaning all atlases must follow DISHNAME_atlas.png structure, otherwise they WILL NOT LOAD.

# soon to be added
-table ordering system in JS

-vertical atlas logic and overall more stable image handling

-monetization options integration such as popup ads,homepage ads...(google ads)
