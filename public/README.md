# What can I do with it?

- Send completely anonymous `messages` or `replies`
    - with `attachments`
        - with `spoilers`
    - and `custom usernames`
    - and `custom PFPs`
        - that are either `statis`: stay same
        - or are `dynamic`: evolve based on usernames 
            - with different selectable styles
- `Report` anonymous messages or replies
- `Ban` users from sending anonymous messages
    - either `automatically` after a set number of `reports`
    - or `manually` by message or reply reference
- Have `Admin Logs`
    - `global`
    - or different for each channel
- Have custom `Anon Profiles`: PFPs and usernames

*Here's a little demo:*
<center><video src="_media/demo1.mp4" type="video/mp4" width="90%" controls playsinline></video></center>

> Whatever latency you saw 👆here while "Sending command..." is due to Discord's slow (file) upload speeds.
> The Anon message is sent back almost instantaneously after the data reaches Anonymity.

> Anonymity, under `no` circumstance, will reveal your true identity to Admins/Moderators. \
> However Admins/Moderators `can` ban you from using Anonymity in their server using [`/user-ban-settings`](#user-ban-settings). \
> Or if you're reported using [`/report-anon-user`](#report-anon-user) more than a set number of times (21 by default), you'll be autobanned from using Anonymity server-wide.

# How do I set it up in my server?

> This section is only for server Admins/Moderators. \
> You at least need the `Kick Members` permission in a server to be considered an Admin/Moderator in that server.

<!-- TODO: complete this section -->

# Concepts and conventions

- ## Anon Usernames


# More for Admins and Moderators


# Commands and behaviour 


- ## `/anon`
    This is Anonymity's main command.

    > Selected channel settings and your usage is shown if both of [`text`](#option-text) and [`attachment`](#option-attachment) options are left empty. 

    - ### option: `text`
        The text you want to send anonymously. \
        This text can be any UTF-8 string. \
        Leave this option empty if you only want to send attachment.

    - ### option: `attachment`
        The attachment you wnat to send anonymously. \
        This attachment can be any of any file type. \
        Leave this option empty if you only want to send text.

    - ### option: `set-attachment-spoiler`
        Set this option to ***True*** if you want to mark the [selected `attachement`](#option-attachment) as spoiler.

        > This option is ignored if [an `attachement`](#option-attachment) is not selected.

    - ### option: `use-custom-profile`
        Set this option to ***True*** if you want to use your 

    - ### option: `message-reply-url`

    - ### option: `channel`
        The channel you want to send anonymous message in.

        > Current channel is selected if this option is left empty.

        > This option is overridden if [`message-reply-url`](#option-message-reply-url) option is selected.

- ## `/my-anon-profile`

    - ### option: `regen-anon-profile`

    - ### option: `set-auto-regen-anon-profile`

    - ### option: `set-custom-username`

    - ### option: `remove-custom-username`

    - ### option: `set-custom-static-pfp-url`

    - ### option: `remove-custom-static-pfp`

    - ### option: `use-custom-profile-by-default`

    - ### option: `delete-custom-profile`

    - ### option: `channel`
        The channel you want to create, modify or delete your Custom Anon Profile for. \
        You may leave this option empty if you want to select the channel you're running this command in.

- ## `/request-handshake`

    - ### option: `anon-username`

- ## `/report-anon-user`

    - ### option: `anon-username`

    - ### option: `reason`

- ## `/server-perks`

    - ### option: `add-to-this-server`

    - ### option: `remove-from-this-server`

    - ### option: `view-details`

- ## `/anonymity-support`


- ## `/send-as-admin`
    > This command is only visible to Admins/Moderators. \
    > You at least need the `Kick Members` permission in a server to be considered an Admin/Moderator in that server.

    > This command is exactly the same as [`/anon`](#anon) except:
    > - Messages or replies sent using this command are not limited to registered channels.
    > - `Admin Logs` show the senders' usernames.
    > - ban by Anon Username does not work on messages or replies sent using this.

    - ### option: `text`

    - ### option: `attachment`

    - ### option: `set-attachment-spoiler`

    - ### option: `use-custom-profile`

    - ### option: `message-reply-url`

    - ### option: `channel`
        The channel you want to send anonymous message in. \
        You may leave this option empty if you want to select the channel you're running this command in.

        > This option is ignored if [`message-reply-url`](#option-message-reply-url) option is selected.

- ## `/anon-channel-settings`
    Register a channel, change channel settings or unregister a channel using this command. \
    To register a channel with default settings, use this command without any options.

    > This command is only visible to Admins/Moderators. \
    > You at least need the `Kick Members` permission in a server to be considered an Admin/Moderator in that server.

    - ### option: `channel`
        The channel you want to register, unregister or change settings of. \
        You may leave this option empty if you want to select the channel you're running this command in.

    - ### option: `set-admin-log-channel`

    - ### option: `remove-admin-log-channel`

    - ### option: `select-dynamic-pfp-style`

    - ### option: `set-slowmode`

    - ### option: `set-reports-to-autoban`

    - ### option: `set-anon-username`

    - ### option: `remove-anon-username`

    - ### option: `set-static-pfp-url`

    - ### option: `remove-static-pfp`

    - ### option: `disable-custom-usernames`

    - ### option: `disable-custom-pfp`

    - ### option: `disable-attachments`

    - ### option: `disable-regen-anon-profile`

    - ### option: `unregister-channel`

- ## `/user-ban-settings`

    > This command is only visible to Admins/Moderators. \
    > You at least need the `Kick Members` permission in a server to be considered an Admin/Moderator in that server.

    - ### option: `anon-username`

    - ### option: `action`

        - #### choice: `ban`

        - #### choice: `unban`

    - ### option: `reason`