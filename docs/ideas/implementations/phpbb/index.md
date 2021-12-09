# PHPBB tables

This page shows some of the PHP Bulletin Board tables.

* [](#)


## acl options

[Link](https://wiki.phpbb.com/Table.phpbb_acl_options)

This table contains the formation which permissions ("can read forum", "can post topics" etc.) are available. See also Permissions.

| column | type (MySQL) | content | default |
| - | - | - | - |
| auth_option_id | mediumint(8) unsigned | primary key | auto_increment |
| auth_option | varchar(50) | the name of the permission, e.g. "f_post" | |
| is_global | tinyint(1) unsigned | this permission can be granted globally (once for all forums) | 0 |
| is_local | tinyint(1) unsigned | this permission can be granted locally (individual setting for each forum) | 0 |
| founder_only | tinyint(1) unsigned | only founders can have this permission | 0 |


## acl roles

[Link](https://wiki.phpbb.com/Table.phpbb_acl_roles)

Permission roles (Standard Moderator, Simple Moderator etc.)

| column | type (MySQL) | content | default |
| - | - | - | - |
| role_id | mediumint(8) unsigned | primary key | auto_increment |
| role_name | varchar(255) | Name of this role, can also be a language string | |
| role_description | text | description of this role, can also be a language | |string | |
| role_type | varchar(10) | tbd | |
| role_order | smallint(4) unsigned | tbd | 0 |


## acl roles data

[Link](https://wiki.phpbb.com/Table.phpbb_acl_roles_data)

This table stores which permissions each role contains

| column | type (MySQL) | content | default |
| - | - | - | - |
| role_id | mediumint(8) unsigned | primary key | 0 |
| auth_option_id | mediumint(8) unsigned | primary key | 0 |
| auth_setting | tinyint(2) | ACL_YES, ACL_NO or ACL_NEVER | 0 |


## acl users

[Link](https://wiki.phpbb.com/Table.phpbb_acl_users)

Permission roles and/or individual permissions assigned to users

| column | type (MySQL) | content | default |
| - | - | - | - |
| user_id | mediumint(8) unsigned | references phpbb_users.user_id | 0 |
| forum_id | mediumint(8) unsigned | references phpbb_forums.forum_id | 0 |
| auth_option_id | mediumint(8) unsigned | references phpbb_acl_options.auth_option_id | 0 |
| auth_role_id | mediumint(8) unsigned | references phpbb_acl_roles.role_id | 0 |
| auth_setting | tinyint(2) | ACL_YES, ACL_NO or ACL_NEVER | 0 |


## acl users

[Link](https://wiki.phpbb.com/Table.phpbb_acl_users)

Permission roles and/or individual permissions assigned to users

| column | type (MySQL) | content | default |
| - | - | - | - |
| user_id | mediumint(8) unsigned | references phpbb_users.user_id | 0 |
| forum_id | mediumint(8) unsigned | references phpbb_forums.forum_id | 0 |
| auth_option_id | mediumint(8) unsigned | references phpbb_acl_options.auth_option_id | 0 |
| auth_role_id | mediumint(8) unsigned | references phpbb_acl_roles.role_id | 0 |
| auth_setting | tinyint(2) | ACL_YES, ACL_NO or ACL_NEVER | 0 |


## bots

[Link](https://wiki.phpbb.com/Table.phpbb_bots)

| column | type (MySQL) | content | default |
| - | - | - | - |
| bot_id | mediumint(8) unsigned | primary key | auto_increment |
| bot_active | tinyint(1) unsigned | tbd | 1 |
| bot_name | varchar(255) | tbd | |
| user_id | mediumint(8) unsigned | tbd | 0 |
| bot_agent | varchar(255) | tbd | |
| bot_ip | varchar(255) | tbd | |


## forums

[Link](https://wiki.phpbb.com/Table.phpbb_forums)

| column | type (MySQL) | content | default |
| - | - | - | - |
| forum_id | mediumint(8) unsigned | primary key | auto_increment |
| parent_id | mediumint(8) unsigned | the forum_id of the parent forum (or category) | 0 |
| left_id | mediumint(8) unsigned | forum_id of the forum left to the current forum in the binary tree (used e. g. to retrieve the list of all parents very fast to create the forum navigation) | 0 |
| right_id | mediumint(8) unsigned | forum_id of the forum right to the current forum in the binary tree (used e. g. to retrieve the list of all parents very fast to create the forum navigation) | 0 |
| forum_parents | mediumtext | Holds an serialized array of parent forums name, id and type, used for generating forum navigation. |
| forum_name | varchar(255) | tbd | |
| forum_desc | text | tbd | |
| forum_desc_bitfield | varchar(255) | see Parsing text | |
| forum_desc_options | int(11) unsigned | see Parsing text | 7 |
| forum_desc_uid | varchar(5) | see Parsing text | |
| forum_link | varchar(255) | tbd | |
| forum_password | varchar(40) | tbd | |
| forum_style | tinyint(4) | tbd | 0 |
| forum_image | varchar(255) | tbd | |
| forum_rules | text | tbd | |
| forum_rules_link | varchar(255) | tbd | |
| forum_rules_bitfield | varchar(255) | see Parsing text | |
| forum_rules_options | int(11) unsigned | see Parsing text | 7 |
| forum_rules_uid | varchar(5) | see Parsing text | |
| forum_topics_per_page | tinyint(4) | tbd | 0 |
| forum_type | tinyint(4) | category (forum_type = FORUM_CAT = 0) or forum (forum_type = FORUM_POST = 1) or link (forum_type = FORUM_LINK = 2) | 0 |
| forum_status | tinyint(4) | tbd | 0 |
| forum_posts | mediumint(8) unsigned | tbd | 0 |
| forum_topics | mediumint(8) unsigned | Number of topics in a forum. | 0 |
| forum_topics_real | mediumint(8) unsigned | Number of topics in a forum. Includes unapproved topics. | 0 |
| forum_last_post_id | mediumint(8) unsigned | tbd | 0 |
| forum_last_poster_id | mediumint(8) unsigned | tbd | 0 |
| forum_last_post_subject | varchar(100) | tbd | |
| forum_last_post_time | int(11) unsigned | tbd | 0 |
| forum_last_poster_name | varchar(255) | tbd | |
| forum_last_poster_colour | varchar(6) | tbd | |
| forum_flags | tinyint(4) | tbd | 32 |
| display_on_index | tinyint(1) unsigned | tbd | 1 |
| enable_indexing | tinyint(1) unsigned | tbd | 1 |
| enable_icons | tinyint(1) unsigned | tbd | 1 |
| enable_prune | tinyint(1) unsigned | tbd | 0 |
| prune_next | int(11) unsigned | tbd | 0 |
| prune_days | tinyint(4) | tbd | 0 |
| prune_viewed | tinyint(4) | tbd | 0 |
| prune_freq | tinyint(4) | tbd | 0 |


## groups

[Link](https://wiki.phpbb.com/Table.phpbb_groups)

| column | type (MySQL) | content | default |
| - | - | - | - |
| group_id | mediumint(8) unsigned | primary key | auto_increment |
| group_type | tinyint(4) | tbd | 1 |
| group_founder_manage | tinyint(1) unsigned | tbd | 0 |
| group_name | varchar(255) | tbd | |
| group_desc | text | tbd | |
| group_desc_bitfield | varchar(255) | tbd | |
| group_desc_options | int(11) unsigned | tbd | 7 |
| group_desc_uid | varchar(5) | tbd | |
| group_display | tinyint(1) unsigned | tbd | 0 |
| group_avatar | varchar(255) | tbd | |
| group_avatar_type | tinyint(4) | tbd | 0 |
| group_avatar_width | tinyint(4) | tbd | 0 |
| group_avatar_height | tinyint(4) | tbd | 0 |
| group_rank | mediumint(8) unsigned | tbd | 0 |
| group_colour | varchar(6) | tbd | |
| group_sig_chars | mediumint(8) unsigned | tbd | 0 |
| group_receive_pm | tinyint(1) unsigned | tbd | 0 |
| group_message_limit | mediumint(8) unsigned | tbd | 0 |
| group_legend | tinyint(1) unsigned | tbd | 1 |


## posts

[Link](https://wiki.phpbb.com/Table.phpbb_posts)

| column | type (MySQL) | content | default |
| - | - | - | - |
| post_id | mediumint(8) unsigned | primary key | auto_increment |
| topic_id | mediumint(8) unsigned | tbd | 0 |
| forum_id | mediumint(8) unsigned | tbd | 0 |
| poster_id | mediumint(8) unsigned | tbd | 0 |
| icon_id | mediumint(8) unsigned | tbd | 0 |
| poster_ip | varchar(40) | tbd | |
| post_time | int(11) unsigned | tbd | 0 |
| post_approved | tinyint(1) unsigned | tbd | 1 |
| post_reported | tinyint(1) unsigned | tbd | 0 |
| enable_bbcode | tinyint(1) unsigned | tbd | 1 |
| enable_smilies | tinyint(1) unsigned | tbd | 1 |
| enable_magic_url | tinyint(1) unsigned | tbd | 1 |
| enable_sig | tinyint(1) unsigned | tbd | 1 |
| post_username | varchar(255) | tbd | |
| post_subject | varchar(100) | tbd | |
| post_text | mediumtext | tbd | |
| post_checksum | varchar(32) | tbd | |
| post_attachment | tinyint(1) unsigned | 1=This post has at least one attachment 0=no attachments in this post | 0 |
| bbcode_bitfield | varchar(255) | see Parsing text | |
| bbcode_uid | varchar(5) | see Parsing text | |
| post_postcount | tinyint(1) unsigned | tbd | 1 |
| post_edit_time | int(11) unsigned | tbd | 0 |
| post_edit_reason | varchar(255) | tbd | |
| post_edit_user | mediumint(8) unsigned | tbd | 0 |
| post_edit_count | smallint(4) unsigned | tbd | 0 |
| post_edit_locked | tinyint(1) unsigned | tbd | 0 |

## topics

[Link](https://wiki.phpbb.com/Table.phpbb_topics)

| column | type (MySQL) | content | default |
| - | - | - | - |
| topic_id | mediumint(8) unsigned | Primary key | auto_increment |
| forum_id | mediumint(8) unsigned | references phpbb_forums.forum_id | 0 |
| icon_id | mediumint(8) unsigned | references phpbb_icons.icon_id | 0 |
| topic_attachment | tinyint(1) unsigned | 1=at least one post in this topic has an attachment 0=no attachments in this topic | 0 |
| topic_approved | tinyint(1) unsigned | Flag indicating whether the topic is awaiting approval or not. | 1 |
| topic_reported | tinyint(1) unsigned | Flag indicating that a post within the topic has been reported. | 0 |
| topic_title | varchar(100) | The title of the topic. | |
| topic_poster | mediumint(8) unsigned | references phpbb_users.user_id | 0 |
| topic_time | int(11) unsigned | Unix timestamp, the topic's creation date. | 0 |
| topic_time_limit | int(11) unsigned | The number of seconds that a topic will remain as a sticky. | 0 |
| topic_views | mediumint(8) unsigned | The number of time the topic has been viewed. | 0 |
| topic_replies | mediumint(8) unsigned | The number of approved replies to this topic. | 0 |
| topic_replies_real | mediumint(8) unsigned | Total number of replies to this topic (including posts waiting for approval). | 0 |
| topic_status | tinyint(3) | ITEM_UNLOCKED(0), ITEM_LOCKED(1) or ITEM_MOVED(2) | 0 |
| topic_type | tinyint(3) | POST_NORMAL(0), POST_STICKY(1), POST_ANNOUNCE(2) or POST_GLOBAL(3) Note that when topic_type is POST_GLOBAL (global announcement), then forum_id must be 0 | 0 |
| topic_first_post_id | mediumint(8) unsigned | references phpbb_posts.post_id | 0 |
| topic_first_poster_name | varchar(255) | The topic creator's username. | |
| topic_first_poster_colour | varchar(6) | The colour of the topic creator's default user group. | |
| topic_last_post_id | mediumint(8) unsigned | references phpbb_posts.post_id | 0 |
| topic_last_poster_id | mediumint(8) unsigned | references phpbb_users.user_id | 0 |
| topic_last_poster_name | varchar(255) | The username of the topic's last poster. | |
| topic_last_poster_colour | varchar(6) | The colour of the last poster's default user group. | |
| topic_last_post_subject | varchar(100) | The subject of the topic's last post | |
| topic_last_post_time | int(11) unsigned | Unix timestamp, the last time a post was made in the topic. | 0 |
| topic_last_view_time | int(11) unsigned | Unix timestamp, the last time the topic was viewed. Used in topic pruning. | 0 |
| topic_moved_id | mediumint(8) unsigned | If topic_status is ITEM_MOVED (a shadow topic), this field contains the topic id of the real topic. | 0 |
| topic_bumped | tinyint(1) unsigned | Has this topic been bumped? 1 (yes), 0(no) | 0 |
| topic_bumper | mediumint(8) unsigned | references phpbb_users.user_id | 0 |
| poll_title | varchar(100) | The poll's question | |
| poll_start | int(11) unsigned | Unix timestamp, poll's creation date | 0 |
| poll_length | int(11) unsigned | Poll duration, in seconds | 0 |
| poll_max_options | tinyint(4) | The number of poll options a user can choose when casting a vote | 1 |
| poll_last_vote | int(11) unsigned | Unix timestamp, time of the last vote | 0 |
| poll_vote_change | tinyint(1) unsigned | Are users allowed to change their vote(s)? 1 (yes), 0(no) | 0 |


## user group

[Link](https://wiki.phpbb.com/Table.phpbb_user_group)

Information about which user is a member/leader or which group.

| column | type (MySQL) | content | default |
| - | - | - | - |
| group_id | mediumint(8) unsigned | references phpbb_groups.group_id | 0 |
| user_id | mediumint(8) unsigned | references phpbb_users.user_id | 0 |
| group_leader | tinyint(1) unsigned | 1 (true) if this user is a group leader | 0 |
| user_pending | tinyint(1) unsigned | 1 (true) if the user is waiting for approval | 1 |
