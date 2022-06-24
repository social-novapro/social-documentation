# A-Class: Developer token error

## A001: Both the developer token and application token were not found

### Description: 

The request is missing both a developer token and an application token. Change the request to include both.



## A002: The developer token was not found

### Description: 

The request is missing a developer token. Change the request to include a developer token.



## A003: The application token was not found

### Description: 

The request is missing an application token. Change the request to include an application token.



## A004: There was no developer token and no application token provided

### Description: 

The request is missing both a developer token and an application token. Change the request to include both.



## A005: There was no provided developer token

### Description: 

The request is missing a developer token. Change the request to include a developer token.



## A006: There was no provided application token

### Description: 

The request is missing an application token. Change the request to include an application token.


# B-Class: User token error



## B001: The user ID provided was not found.

### Description: 

The user ID provided could not be found. Check that the user ID is valid and try again.



## B002: The user token provided did not match the provided user ID's user token, and the access token provided did not match the access token for the user token and app token.

### Description: 

The user token provided did not match the user token associated with the provided user ID, and the access token provided did not match the access token associated with the user token and app token. Check that the user token and access token are valid and try again.



## B003: The user token provided did not match the provided user ID.

### Description: 

The user token provided did not match the user token associated with the provided user ID. Check that the user token is valid and try again.



## B004: The access token provided did not match the access token for the provided user token, app token, and user ID.

### Description: 

The access token provided did not match the access token associated with the provided user token, app token, and user ID. Check that the access token is valid and try again.



## B005: There was no user ID, user token or access token provided.

### Description: 

The request is missing a user ID, user token, and access token. Change the request so that it includes all three.



## B006: There was no user ID or user token provided.

### Description: 

The request is missing a user ID and user token. Change the request so that it includes both.



## B007: There was no user ID or access token provided.

### Description: 

The request is missing a user ID and access token. Change the request so that it includes both.



## B008: There was no user token or access token provided.

### Description: 

The request is missing a user token and access token. Change the request so that it includes both.



## B009: There was no user ID provided.

### Description: 

The request is missing a user ID. Change the request so that it includes the user's UUID.



## B010: There was no user token provided.

### Description: 

The request is missing a user token. Change the request so that it includes the user's token.



## B011: There was no access token provided.

### Description: 

The request is missing an access token. Change the request so that it includes the access token.



## B012: The username provided was not found.

### Description: 

The username provided could not be found. Check that the username is valid and try again.



## B013: The user ID provided was not found in the private schema.

### Description: 

The user ID provided could not be found in the private schema. Check that the user ID is valid and try again.

# C-Class: User data error

## C001: The requested username has already been used.

### Description: 

A user with the same username already exists. Choose a different username.



## C002: You must provide the new user's username and displayName in order to create a user.

### Description: 

The request is missing either the username or displayName. Change the request so that it includes both.



## C003: You must provide the new user's username in order to create a user.

### Description: 

The request is missing the username. Change the request so that it includes the desired username.



## C004: You must provide the new user's displayName in order to create a user.

### Description: 

The request is missing the displayName. Change the request so that it includes the desired displayName.



## C005: There were no users found.

### Description: 

No users were found that match the specified criteria.


# D-Class: Post data error

## D001: The provided post ID is not valid. It was either deleted or does not exist.

### Description: 

The post ID is not valid. Check that the post still exists, and that the ID is correct.



## D002: There was an error trying to find the post data.

### Description: 

There was an error when trying to find the post data. Try again later.



## D003: There were no posts found.

### Description: 

There were no posts found. Check the parameters of the request, and try again.

# E-Class: Authentication error

## E001: You must provide post content and a user ID to submit a post.

### Description: 

The request is missing both content and a user ID. Change the request so that it includes both.



## E002: You must provide post content submit a post.

### Description: 

The request is missing content. Change the request so that it includes text and/or images.



## E003: You must provide a user ID to submit a post.

### Description: 

The request is missing a user ID. Change the request so that it includes the user's UUID.



## E004: Forbidden, please have the user sign in again! The provided info was not correct!

### Description: 

The request was performed with an expired token. Sign in again to refresh the token, then try again.



## E005: The provided post length is over 512 characters. 

### Description:

The request was performed with too many characters. Shorten the text length and try again.



## E006: The provided content has over 10 newlines.

### Description:

The request, after line wraps, spans over 10 lines. Shorten the content so that it fits within 10 lines and try again.



## E007: The provided developer token was not found.

### Description:

The developer token given could not be found. Try regenerating the token.



## E008: There was no provided developer token.

### Description: 

The request did not come with a developer token. Include one and try again.



## E009: The User ID provided in the header is not the same as the User ID in the body.

### Description:

The request contains mismatching User IDs in the header and body. Change your request so the User IDs match.
