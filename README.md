# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
StegExpose and File Signature Analysis Commands

## OUTPUT:
- **1.Install and Set Up StegExpose**
• Download the StegExpose .jar file from the official repository.
• Ensure Java Runtime Environment (JRE) is installed.
• Run the tool on an image or a folder of images:\

• The output will list detection scores and a "suspect" verdict if steganography
is found.

- **2.Scan Individual Files**
• Run StegExpose on a single image:

The tool uses statistical analysis methods like RS analysis, Sample Pair
analysis, and Chi-square attack to detect hidden content.

- **3.Analyze File Signatures**
• Use Linux commands to verify the file's true format:

Every file type has a magic number (e.g., JPEG files start with FFD8). Comparing
the actual signature with the file extension helps identify mismatches or embedded
file tricks.

- **4. Cross-Check File Behavior**
• Rename the file (e.g., mv suspicious.jpg suspicious.zip) and try extracting it:

o Sometimes, files are disguised (e.g., a ZIP file hidden as a JPG), and this
trick helps uncover such embedded archives.

- **5.Optional: Use Other Tools**

o Tools like binwalk, stegsolve, or zsteg can be used for deeper analysis,
especially for PNG files or binary dumps.

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/694863a0-2118-4c73-a1a3-9c582fbeddc4" />


<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/02600996-ff35-4726-99f3-3448b8eefa7d" />

<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/88818aba-74a0-4b68-a3d2-27956984e887" />


<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a0adb75f-880c-4870-ad40-a6c5784ed2b7" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5458b496-e1fd-4721-b9fb-9bb2f96fdb1b" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/96a7559e-bc7f-4b80-915a-e252a7600962" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1c1c4ba5-4cf5-4631-a877-edbc6d20ed33" />


## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
