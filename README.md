# Content Styling

## What is this?

This is my attempt to make this content:

- https://www.urmc.rochester.edu/encyclopedia/content.aspx?ContentID=4552&ContentTypeID=1

Look amazing 😍

To do this I'm using:

- https://andy-bell.co.uk/a-modern-css-reset/
- https://set.studio/some-simple-ways-to-make-content-look-good/
- https://andy-bell.co.uk/my-favourite-3-lines-of-css/

## Notes

- Use Type Scales (this one uses Third Major)
    - https://typescale.com/
- Use Utopia for creating more flud typer scales
    - https://utopia.fyi/


## Steps

- Get semantic HTML markup (droper use of div, p, headings, list, and blockquote tags)
- Reset your CSS using a simple reset
- Set some foundational items (background, text color, body padding)
    - Use `:root{}` vars for colors
- Set type scales 
    - See: https://typescale.com/
- Apply type scales to body, heading, and blockquote elements
- Keep it going...

## Deployment

- Deployed through `flyctl` using Docker which is medium lame...
- If you are interested in building it locally do this
    - `docker build -t content-styling . && docker run -p 8043:8043 content-styling`
- Otherwise init the project 
    - `flyctl launch`
- Modify the _fly.toml_ to properly map the port
    - `internal_port = 8043`
- Deploy the app
    - `flyctl deploy`
- View the app
    - `flyctl open`