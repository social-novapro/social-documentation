# interactThemeSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | themeID |
| userID | string | true | who created the theme |
| indexID | string | true | index id |
| theme_name | string | true | name for theme |
| timestamp | number | true | time created |
| timestamp_edited | number | true | time edited |
| locked | boolean | true | is theme locked |
| theme_fork | string | false | theme forked from |
| privacy | number | true | 1: public, 2: friends of friends, 3: private |
| colourTheme | [colourThemeSchema](#colourthemeschema) | true | colour theme |

## colourThemeSchema
| Field | Type | Required | Description |
| -- | -- | -- | -- |
| _id | string | true | id of theme, themeID |
| posts | string | false | colour of posts |
| font_posts_content | string | false | font of posts content |
| font_posts_action | string | false | font of posts action |
| background | string | false | background colour |
| navigation | string | false | colour of navigation |
| font_navigation | string | false | font of navigation |
| navSecondary | string | false | colour of secondary navigation |
| font_navSecondary | string | false | font of secondary navigation |
| menu | string | false | colour of menu |
| font_menu | string | false | font of menu |
| menuButton | string | false | colour of menu button |
| font_menuButton | string | false | font of menu button |
| font_h1 | string | false | font of h1 |
| font_otherUser | string | false | font of other user |
| font_ownUser | string | false | font of own user |
| font_p_secondary | string | false | font of secondary p |
