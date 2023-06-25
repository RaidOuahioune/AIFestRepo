# Data cleaning

#### Things to consider

- **Booking Lead Time**: convert units

- **Arrival Date Year**: check sanity

- **Arrival Date Month**: check sanity

- **Arrival Date Week Number**: 
  
  - check if week lies inside the given month
  
  - <= 53
  
  - positive

- **Arrival Date Month Day**:  0 < m_day <= 31

- **Weekends Stays**: 
  
  - 0 <= w_d <= 2

- **Weekdays Stays**: other than weekend nights

- **Wisymurfs**: max 10

- **Smurflings**: max 12

- **Babies Number**: max 12

- **Meal Type**: BB means Bed & Breakfast

- **Smurfland**: 3 chars

- **Market Segment**: 

- ![](assets/2023-06-18-14-03-22-image.png)

**Booking Channel**:

        ![](assets/2023-06-18-14-03-45-image.png)

- **Smurfy smurf**: 0/1

- **Previous Cancellations Number**: number >= 0

- **Request Mushroom Type**: one character

- **Allocated Mushroom Type**: 
  
  - one character.
  
  - create feature to detect if the requested type is the same as the allocated one

- **Booking Changes**: number
  
  - **Deposit Type**: 
    
    ![](assets/2023-06-18-14-08-46-image.png)

- **Agent**: ID  (will probably drop)

- **Moberry**: ID  (discuss dropping)

- **Days in Waiting List**: number (prolly has high correlation)

- **Customer Type**:
  
  ![](assets/2023-06-18-14-11-47-image.png)











### data formats

- meal_type:    <mark>TODO</mark>
  
  - 1 letters of initials capital

- smurfland:
  
  - 3 chars

- market_segment:    <mark>TODO</mark>
  
  - convert all to capital

- booking_channel:   <mark>TODO</mark>
  
  - take capitalized initials only

- smurfy_smurf:
  
  - 0/1

- number_of_previous_cancellations:

- previous_bookings_not_canceled:

- **total_bookings**: engineered

- **most likely to cancel**: boolean (cancel = max(cancel, previous))?

- Request Mushroom Type: one character​   DONE

- Allocated Mushroom Type:  DONE
  
  - one character.

- **got_requested_mushroom** boolean (engineered)

- booking_changes: num

- deposit_type:    <mark>TODO</mark>
  
  - capitalize all

- moberry: drop

- customer_type: Initials (SS, SP, L, S)    <mark>TODO</mark>

- average_daily_rate:

- **total_stayed_days**: 

- **sum of all lodging transactions**: 

- mushotel_location: dropped





format uniformization / data formatting
