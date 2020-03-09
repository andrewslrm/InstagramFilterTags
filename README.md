# InstagramFilterTags
Functions that filter media post at Instagram by tag or array tags


## Examples

### Filter media posts by only one hastag

- The **accountId** is not the user name, the accountId is a number and get in [https://codeofaninja.com/tools/find-instagram-user-id](https://codeofaninja.com/tools/find-instagram-user-id).
- The **tag** is a string with the character # requied
 


```javascript

import { getInstagramMediaByTag } from './src/instagram';

const fetchMedia = async () => {
    const mediaItems = await getInstagramMediaByTag(4540911, '#8m');
    console.log(mediaItems)
}

```


### Filter multiple media posts with tags

- The ***accountId** is not the user name, the accountId is a number and get in [https://codeofaninja.com/tools/find-instagram-user-id](https://codeofaninja.com/tools/find-instagram-user-id).
- The **listTags** is a string array with the hashtag to search, the character # is required in the tags
 


```javascript

import { getInstagramMediaByListTags } from './src/instagram';

const fetchMedia = async () => {
    const mediaItems = await getInstagramMediaByListTags(4540911, ['#8m', '#turtle', '#cdmx']);
    console.log(mediaItems)
}

```


