# Different Network Publisher

## Summary
Publisher is part of a bigger project called Different Network. It is a desktop application that does all the processing necessary to generate necessary data or files for the content to be published to DN, files like converting images to webp and generating lazy images and data like extracting colors for all the images used for later use in placeholders. Publisher is developed using Electron.js, React.js and Postgres.

## How it works
After the writer file is imported, the data it provides gets validated, as well as the assets it points to, meaning it checks for their existence, validates their dimensions, aspect ratio, format... Then from does assets lazy images, and next gen formats like webp, the image swatch are extracted. Once the validation and extraction is done an

When DN Publisher is opened a blank card appears.

![Different Network Publisher Init](/public/assets/1.png)

Then by pressing ctrl + o you can choose a writer file to import. Publisher will proceed to validate the file and extract data from it and generate other relevant data itself. The title, the post type, the assets, the size of each asset, asset colors... The background image/video is taken from the assets and will prioritize a video if it exists in the assets.

![Different Network Publisher Imported](/public/assets/2.png)

You can start uploading the assets to the CDN buy pressing the upload button. After the upload is done, a publish button will appear that publishes everything to the website.

![Different Network Publisher Uploading](/public/assets/3.png)

## Gif Demo

![Different Network Publisher](/public/assets/dnp.gif)