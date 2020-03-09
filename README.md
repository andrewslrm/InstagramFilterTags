# InstagramFilterTags
Functions that filter media post at Instagram by tag or array tags


## Examples

### Filter post by only one hastag

- The accountId is not the user name, the accountId is a number and get in [https://codeofaninja.com/tools/find-instagram-user-id](https://codeofaninja.com/tools/find-instagram-user-id).
- The tag is a string with the character # requied
 


```javascript

import { getInstagramMediaByTag } from './src/instagram';

const fetchMedia = async () => {
    const mediaItems = await getInstagramMediaByTag(4540911, '#8m');
    console.log(mediaItems)
}

```
