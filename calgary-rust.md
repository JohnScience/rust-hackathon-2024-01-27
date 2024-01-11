# Booking rooms for events

One part of organizing an in-person event is booking a room for it. While Calgary Rust isn't too big, we still can book a room in the Central Library for our events at no cost. However, this requires some manual work.

## Process

### Booking a room

1. First, we go to <https://calgarylibrary.ca/events-and-programs/book-a-space/book-a-room/>.
2. Then, we pick a date to see the available rooms.
3. After that, we have to select a room based on the number of people who are going to attend the event.

<details>
  <summary>Room space considerations</summary>

Rooms like `2-05A Meeting Room`, `2-05B Meeting Room`, `2-05C Meeting Room`, and `3-10A Meeting Room` can accommodate up to 10 people.

Rooms like `3-20A Idea Lab`, `3-10B Meeting Room` can accommodate up to 16 people.

Note that some rooms like `3-10C Teen Study Hall` and `3-10D Teen Tech Lab` should not be used for our events.

Right now, we can dispense with rooms that can accomodate only 10 people but I can foresee that we will need to book a room for 16 people rather soon.

After that, we'll probably need to request help from Central Library, InceptionU, Platform Calgary, or Microsoft to book even bigger rooms.

</details>

4. Then, we have to manually click on the "View Availability" button for each room to see if it's available on the date we want and to see the time slots that are available for that room.

<details>
  <summary>Booking time considerations</summary>

Time slots are time moments separated by 30-minutes intervals. There will be at least 2 time slots available for each room - the beginning and the end (e.g. `9:00` and `9:30`, which correspond to a 30-minute-long span). Usually, the number of blocks is under 10. The number of blocks is tied to the working hours of the Central Library, which can vary depending on the time of the day.

Our goal is to have at least 1h30m for the event. This means that we need to book at least 4 time slots (e.g. `9:00`, `9:30`, `10:00`, and `10:30`).

Ideally,

* the event shouldn't coincide or happen close to the same time with other events in Calgary.
* the event days should alternate between weekdays and weekends.
* the event should be scheduled before Tony Grimes from Pixels YYC announces the upcoming events.

</details>

5. Once the room and the time slots are chosen, we have to fill out the form which prompts us to enter (1) the meeting title, (2) username or barcode, and (3) PIN of the library card.

After the form is submitted, the room is booked.

### Publish the event

After the room is booked, we have to publish the event on Meetup and Eventbrite. It involves filling out numerous forms and copying and pasting the same information over and over again.

Further description is TBD.

### Announcing the event

After the event is scheduled, we have to announce it...

* In [Calgary Rust Discord server](https://discord.gg/N2vzPeADzn).
* To Tony Grimes from Pixels YYC (perhaps, via a mention in the message in the Calgaru Rust Discord server).
* Platform Calgary (see <https://www.platformcalgary.com/events/submit>).
* To the [In The Know YYC](https://kettera.apps.ca-1a.mendixcloud.com/p/InTheKnowYYC).
* Other platforms.

## Possibly useful technologies

Most likely, we'll need a headless browser to automate the process of booking a room. You can consider using <https://github.com/rust-headless-chrome/rust-headless-chrome> or <https://github.com/jonhoo/fantoccini>. Going with `fantoccini` is preferrable because it's based on WebDriver protocol and can be used with other browsers.

For asynchronicity, it's recommended to use [`tokio`](https://tokio.rs/tokio/tutorial).
