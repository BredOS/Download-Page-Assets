# Download-Page-Assets
## Format for the boards
```json
"board_name": {
  "name": "",
  "image": "",
  "board_description": "",
  "download_links": {
    "latest": {
      "name": "",
      "link": "",
      "check_sum": ""
    }
  }
}
```
### Board name
`board_name` is just a placeholder value for what board will be linked in the website. This would be easy for the javascript that will be implemented to handle and update the downloads for the website. 
### Name the board!!
`name` in the structor will be used as the title text in the info page for the downloads. 
### Image!
`images` will store the image location that you will want to display. This may be changed to `device_image`|String| later.
### Descriptions!
`board_description` stores the sting of what the board is. Be mindful new lines will need the html new line tag.
### Download links!
`download_links` is an array that holds the container for images/builds of BredOS for the board.
#### Latest link
Make sure `latest` is the latest, but dont forget to make the old latest it's own link contaner and please dont remove it if older versions are needed.
#### Link name
Like `name` in board the `name` in the link container will display on the site.
#### Checksums
The `check_sum` is for the image/build just in case people worry, but it's optional. Leave it an empty string if we don't have one.
