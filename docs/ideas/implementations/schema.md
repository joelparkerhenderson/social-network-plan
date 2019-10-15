# Schema

Schema examples from open source projects.


### Schema models by Open Event Server

https://github.com/fossasia/open-event-server/tree/development/app/api/schema

Models:

   * access_code
   * activity
   * base
   * custom_form
   * custom_form_option
   * custom_placeholder
   * custom_system_role
   * discount_code
   * email_notification
   * event
   * event_copyright
   * event_invoice
   * event_location
   * event_orga
   * event_sub_topic
   * event_topic
   * event_type
   * export_job
   * faq
   * faq_type
   * feedback
   * image_size
   * import_job
   * invite
   * mail
   * message_setting
   * microlocation
   * module
   * notification
   * order
   * page
   * panel_permission
   * permission
   * role
   * role_invite
   * service
   * session
   * session_speaker_link
   * session_type
   * setting
   * social_link
   * speaker
   * speakers_call
   * sponsor
   * stripe_authorization
   * tax
   * ticket
   * ticket_fee
   * ticket_holder
   * track
   * user
   * user_email
   * user_favourite_event
   * user_permission
   * user_token_blacklist
   * users_events_role
   * version

### Schema by OnRuby

https://github.com/phoet/on_ruby/blob/master/db/schema.rb

```ruby
ActiveRecord::Schema.define(version: 2019_05_15_101441) do

  # These are extensions that must be enabled in order to support this database
  enable_extension "plpgsql"

  create_table "authorizations", id: :serial, force: :cascade do |t|
    t.string "provider"
    t.string "uid"
    t.integer "user_id"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.index ["user_id"], name: "index_authorizations_on_user_id"
  end

  create_table "events", id: :serial, force: :cascade do |t|
    t.string "name"
    t.datetime "date"
    t.text "description"
    t.integer "location_id"
    t.integer "user_id"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.boolean "published"
    t.string "label", default: "hamburg"
    t.integer "limit"
    t.integer "github_issue"
    t.index ["location_id"], name: "index_events_on_location_id"
    t.index ["user_id"], name: "index_events_on_user_id"
  end

  create_table "highlights", id: :serial, force: :cascade do |t|
    t.string "description"
    t.string "url"
    t.datetime "start_at"
    t.datetime "end_at"
    t.datetime "created_at", null: false
    t.datetime "updated_at", null: false
    t.string "label", default: "hamburg"
  end

  create_table "jobs", id: :serial, force: :cascade do |t|
    t.string "name"
    t.string "url"
    t.integer "location_id"
    t.datetime "created_at", null: false
    t.datetime "updated_at", null: false
    t.string "label", default: "hamburg"
    t.index ["location_id"], name: "index_jobs_on_location_id"
  end

  create_table "likes", id: :serial, force: :cascade do |t|
    t.integer "user_id"
    t.integer "topic_id"
    t.datetime "created_at", null: false
    t.datetime "updated_at", null: false
  end

  create_table "locations", id: :serial, force: :cascade do |t|
    t.string "name"
    t.string "url"
    t.string "street"
    t.string "house_number"
    t.string "city"
    t.string "zip"
    t.float "lat"
    t.float "long"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.boolean "company"
    t.string "label", default: "hamburg"
    t.string "wheelmap_id"
    t.index ["id"], name: "index_locations_on_id"
  end

  create_table "materials", id: :serial, force: :cascade do |t|
    t.string "name"
    t.text "description"
    t.string "url"
    t.integer "user_id"
    t.integer "event_id"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.string "preview_type"
    t.string "preview_code"
    t.integer "topic_id"
    t.index ["event_id"], name: "index_materials_on_event_id"
    t.index ["user_id"], name: "index_materials_on_user_id"
  end

  create_table "participants", id: :serial, force: :cascade do |t|
    t.integer "user_id"
    t.integer "event_id"
    t.boolean "maybe"
    t.text "comment"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.index ["event_id"], name: "index_participants_on_event_id"
    t.index ["user_id"], name: "index_participants_on_user_id"
  end

  create_table "topics", id: :serial, force: :cascade do |t|
    t.string "name"
    t.text "description"
    t.integer "user_id"
    t.integer "event_id"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.string "label", default: "hamburg"
    t.string "proposal_type", default: "proposal"
    t.integer "github_issue"
    t.index ["event_id"], name: "index_topics_on_event_id"
    t.index ["user_id"], name: "index_topics_on_user_id"
  end

  create_table "users", id: :serial, force: :cascade do |t|
    t.string "nickname"
    t.string "name"
    t.string "image"
    t.string "url"
    t.string "location"
    t.text "description"
    t.datetime "created_at"
    t.datetime "updated_at"
    t.string "github"
    t.boolean "admin"
    t.boolean "freelancer"
    t.boolean "available"
    t.boolean "hide_jobs", default: false
    t.string "twitter"
    t.string "email"
    t.boolean "super_admin", default: false
    t.string "linkedin"
    t.index ["nickname"], name: "index_users_on_nickname", unique: true
  end

end
```