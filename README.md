# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
- **Installation :**
  ```bash
   sudo apt update
   sudo apt install exiftool -y
   sudo apt install plaso -y
   sudo apt install steghide -y
   sudo apt install binwalk -y
 ```
- **📂 Extract metadata from a file:**
  ```bash
  exiftool example.png
  exiftool jpg.jpeg
  ```
- **Embed data**
  ```
  steghide embed -cf (image path) -ef (text file path)
  steghide embed -cf /home/bharathi/Downloads/png.jpeg -ef /home/bharathi/Downloads/hidden.txt
  ```
- **Extract hidden data:**
  ```
  steghide extract -sf (imamge path)
  steghide extract -sf png.jpeg
  ```
- **Using binwalk – for file analysis**  
  ```bash
   binwalk png.jpeg
  ```

  
## OUTPUT:

### Extraction of Metadata using exiftool
![image](https://github.com/user-attachments/assets/2c8f9618-2705-4df6-b33c-93485727bbb8)

### Data Embedding in Image
![image](https://github.com/user-attachments/assets/f7f7a96c-a17a-4d59-be5c-59f2a6b635f7)

### Extraction of hidden data
![image](https://github.com/user-attachments/assets/a165de2f-8dd7-4b68-9a73-5ee22e17c146)

### Using binwalk – for file analysis
![image](https://github.com/user-attachments/assets/a723de55-b99c-44d3-b3fa-4a843a2302cd)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

