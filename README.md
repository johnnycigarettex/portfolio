# Johnny Cigarette portfolio site

## Project Details
- Project live at http://johnnycigarette.ie/
- Site hosted on GitHub pages through this account
- Any file edits will auto deploy live to site
- Domain registed with Black Knight
  - Login - https://www.blacknight.com/
  - Name - johnnycigarettex 
  - Pass - D**!

## How to update the site

### Edit the text on the site
- In the list fo files above, open `siteContent.json`
- Here is the all the text content currently on the site
- Click the pencil icon in the top right to edit
- For additonal formatting you can:
  - Add italic text with `<em> Italic text </em>`
  - Add bold text with `<strong> Bold text </strong>`
  - Add a link with `<a href=\"wwww.linkwebsite.com\"> Link text </a>`
- If you want to add a double quote to a piece of text (") make sure to add a back slash before it (\") so it doesn't break the page
- Once finished click the green `Commit changes` button at the bottom of the page
- If you want, you can copy-paste the file contents into 'https://jsonlint.com/' to make sure its all formtted correctly

### Edit / upload images
- In the list of files above, open the folder `images`
- In the top right, click `Add file`
- Once the file is uploaded, open and edit `siteContent.json` (see above)
- Find the page you want to add the new image to
- Add the image name to the list of images
  ```
     "images": [
        "trinity_1.gif",
        "trinity_2.gif",
        "new_image_name.gif"
      ]
  ```
- Ensure the file name (including the file type extension) matches the uploaded file
- Ensure the name is surrounded by double quotes (")
- Ensure there is a comma at the end of each file name in the list, except for the last one, as shown above
- If you want, you can copy-paste the file contents into 'https://jsonlint.com/' to make sure its all formtted correctly

### Add a new page
- Edit the `siteContent.json` file (see above)
- Each of the sections "Animaton", "Illustration", and "Shop" listed here has a list of pages.
- Each page is between curly brackets in the format:
  ```
    {
      "title": "Page title",
      "text": "Page intro text",
      "videoLink": "video embed link",
      "images": [
        "image_1.gif",
        "image_2.gif"
      ]
    },
  ```
- The fields `"text"`, `"videoLink"` and `"images"` are all optional, and aren't needed on every page
- To add a new page, copy and paste one of the exisiting pages, and then edit the fields as needed (see sections above)
- Ensure that for each page, there is a comma after the last curly bracket, except for the last page in the section
- If you want, you can copy-paste the file contents into 'https://jsonlint.com/' to make sure its all formtted correctly

### Add an embeded video
- To embed a video from YouTube, add the embeded link as the `"videoLink"` parameter of the page
- This link will always be `https://www.youtube.com/embed/` followed by the video's id
- You can get this id on the video's YouTube page - its everything after `v=` in the url
- For example, for the video `https://www.youtube.com/watch?v=YH_X1AkOYjM`, the id is `YH_X1AkOYjM` and the embed link is `https://www.youtube.com/embed/YH_X1AkOYjM`
- For Vimeo, its mostly the same - the link will always be `https://player.vimeo.com/video/` followed by the video's id
- On Vimeo, this is everything after the first slash in the url - for `https://vimeo.com/501737344` its `501737344`
- If you want, you can copy-paste the file contents into 'https://jsonlint.com/' to make sure its all formtted correctly