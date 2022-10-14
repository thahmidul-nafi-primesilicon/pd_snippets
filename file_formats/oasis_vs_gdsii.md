### GDSII (Graphic Design System II)

[] Is in Binary Format
[] Contains:
		[] Layers
		[] Geometry shapes
		[] Text Labels
[] Large files in the order of 100 gigabytes or terabytes
[] Compression doesn't help a lot, uncompressing also takes a lot of time
[] Loading and processing time is huge.
[] Data length is fixed to 32 bits (not adequate for nanoscale structures on 300mm wafers)
[] Link <a href ="https://www.artwork.com/gdsii/gdsii/"> GDSII File Descriptions	</a>
[] De facto industry standard
[] Final file that is sent to the foundry
### OASIS

[] Is also in Binary format, But with variable data length
[] Thus adequate for even nanoscale structures of 300mm wafers
[] Contains similar information to GDSII
[] Much smaller file size compared to GDSII due to intelligent compression strategies
[] Recognizes complex pattern in data and saves them as individual instances or geometry objects
[] Compared to conventional gzip, OASIS CBLOCKS compress the individual cells within the layout
[] Files do not need to be temporarily uncompressed and can be unzipped in parallel
[] To save loading time, it contains a lookup table containing the location of different cells within the file 
[] Also the final file sent to foundry

