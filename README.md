# Home Owner Management Program

## Overview

This program will allow the Home Owner Association to manage all of the subdivision member information, monthly dues collection, event promotion/announcement, amenities concern, overall budget accounting.

### Use Cases

#### HOA Officer POV

1. Add/Update/Delete/Display home/unit owner information.
2. Add/Update/Delete/Display home/unit owner current occupant member information.
3. Add/Update/Delete/Display home/unit owner vehicle information.
4. Add/Update/Delete/Display subdivision fund transaction.
5. Add/Update/Delete/Display subdivision event promotion/announcement.
6. Add/Update/Delete/Display subdivision visitor information.
7. Add/Update/Delete/Display home/unit owner pet information.

### Database Schema

#### Tables:

- owner
  - id
  - firstname
  - middlename
  - lastname
  - age
  - gender
  - birthday (Optional)
  - unit_number
  - unit_block
  - unit_lot
  - unit_street
  - telephone_number
  - mobile_number
  - social_media
  - move_in_date
  - insert_datetime
  - update_datetime
  - Notes
- vehicle
  - id
  - owner_id
  - type ("tricycle", "4-wheel", "e-bike", "motorcycle", "scooter", "bike", "other")
  - brand
  - picture
  - plate number (optional)
  - color
  - with_parking ("True")
  - insert_datetime
  - update_datetime
- occupant
  - id
  - firstname
  - middlename (Optional)
  - lastname
  - age
  - gender
  - insert_datetime
  - update_datetime
- fund
  - id
  - new_balance
  - prev_balance
  - type ("income", "expense")
  - transaction_type_id
  - insert_datetime
  - update_datetime
- pet
  - id
  - name
  - type ("dog", "cat")
  - breed (optional)
  - color
  - owner_id
  - insert_datetime
  - update_datetime
- visitor
  - id
  - name
  - owner_id
  - purpose
  - time_in
  - time_out
  - ticket_number
  - id_provided
  - id_picture
  - plate_number (Optional)
  - count
  - insert_datetime
  - update_datetime

## Backend Task

- Create API that perform the following
  - CRUD owner information.
  - CRUD vehicle information.
  - CRUD occupant information.
  - CRUD fund transaction.
  - CRUD pet information.
  - CRUD visitor information.

## Frontend Task

- Create UI Prototype of the following page:
  - Home page
  - Login Page
  - CRUD owner information.
  - Announcement Page
  - Subdivision Map
  - Home Owners Rules/Mission/Vision
  - CRUD vehicle information.
  - CRUD occupant information.
  - CRUD fund transaction.
  - CRUD pet information.
  - CRUD visitor information.

## TechStack to be used:

- Backend
  - Python Django Rest Framework for the API
  - Database PostgreSQL/ SQL Lite.
  - pytest unit test
- Frontend
  - React JS + Typescript.
- Deployment
  - Vercel

## Future features

- Integrated CCTV Live feed in the website.
- Automatic visitor car parking assignment.
- Adding owners business registration and community section.
