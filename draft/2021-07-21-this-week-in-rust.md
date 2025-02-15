Title: This Week in Rust 400
Number: 400
Date: 2021-07-21
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a programming language empowering everyone to build reliable and efficient software.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

## Updates from Rust Community

### Official

### Newsletters

### Project/Tooling Updates

* [Franzplot: a teaching software (re)written in Rust](https://gfx-rs.github.io/stories/franzplot.html)
* [wgpu: release of v0.9 and the future](https://gfx-rs.github.io/2021/07/16/release-0.9-future.html)

### Observations/Thoughts

 - [Compiling Rust is NP-hard](https://niedzejkob.p4.team/rust-np/)
 - [How we improved the performance of our Rust app](https://www.poor.dev/blog/performance/)

### Rust Walkthroughs

* [Host a Wasm module easily on Raspberry Pi Part 2](https://blog.knoldus.com/host-a-wasm-module-easily-on-raspberry-pi-part-2/)

### Papers

### Miscellaneous


## Crate of the Week

This week's crate is [endbasic](https://www.endbasic.dev), an emulator friendly DOS / BASIC environment running on small hardware and the web.

Thanks to [Julio Merino](https://users.rust-lang.org/t/crate-of-the-week/2704/935) for the suggestion.

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [Knurling-rs user survey](https://forms.office.com/r/aMfHG79N9K)

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Updates from Rust Core

254 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-07-05..2021-07-12

* [improve opaque pointers support](https://github.com/rust-lang/rust/pull/86873)
* [recover from `&dyn mut` ... parse errors](https://github.com/rust-lang/rust/pull/86812)
* [improve error reporting for modifications behind `&` references](https://github.com/rust-lang/rust/pull/86815)
* [do not suggest adding a semicolon after ?](https://github.com/rust-lang/rust/pull/87061)
* [use `#[track_caller]` in const panic diagnostics](https://github.com/rust-lang/rust/pull/87000)
* [query-ify global limit attribute handling](https://github.com/rust-lang/rust/pull/86674)
* [support forwarding caller location through trait object method call](https://github.com/rust-lang/rust/pull/81360)
* [shrink the deprecated span](https://github.com/rust-lang/rust/pull/86320)
* [report an error if resolution of closure call functions failed](https://github.com/rust-lang/rust/pull/86249)
* [stabilize `RangeFrom` patterns in 1.55](https://github.com/rust-lang/rust/pull/83918)
* [account for capture kind in auto traits migration](https://github.com/rust-lang/rust/pull/86869)
* [stop generating `alloca`s & `memcmp` for simple short array equality](https://github.com/rust-lang/rust/pull/85828)
* [inline `Iterator as IntoIterator`](https://github.com/rust-lang/rust/pull/84560)
* [optimize unchecked indexing into `chunks` and 'chunks_mut`](https://github.com/rust-lang/rust/pull/86823)
* [add `Integer::log` variants](https://github.com/rust-lang/rust/pull/80918)
* [special case for integer log10](https://github.com/rust-lang/rust/pull/869309)
* [cargo: unify cargo and rustc's error reporting](https://github.com/rust-lang/cargo/pull/9655)
* [rustdoc: fix rendering of reexported macros 2.0 and fix visibility of reexported items](https://github.com/rust-lang/rust/pull/86841)

### Rust Compiler Performance Triage

Mostly quiet week; improvements outweighed regressions.

Triage done by **@simulacrum**.
Revision range: [9a27044f4..5aff6dd](https://perf.rust-lang.org/?start=9a27044f42ace9eb652781b53f598e25d4e7e918&end=5aff6dd07a562a2cba3c57fc3460a72acb6bef46&absolute=false&stat=instructions%3Au)

1 Regressions, 4 Improvements, 0 Mixed; 0 of them in rollups

[Full report here](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-07-13.md).

### Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [RFC: I/O Safety](https://github.com/rust-lang/rfcs/pull/3128)

### Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

*No RFCs are currently in the final comment period.*

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Move assert_matches to an inner module](https://github.com/rust-lang/rust/pull/86947)
* [disposition: merge] [Stabilize arbitrary_enum_discriminant](https://github.com/rust-lang/rust/pull/86860)
* [disposition: close] [regression: infallible residual could not convert error](https://github.com/rust-lang/rust/issues/86831)
* [disposition: merge] [Document iteration order of retain functions](https://github.com/rust-lang/rust/pull/86790)
* [disposition: merge] [Partially stabilize const_slice_first_last](https://github.com/rust-lang/rust/pull/86593)
* [disposition: merge] [Stabilize const_fn_transmute, const_fn_union](https://github.com/rust-lang/rust/pull/85769)
* [disposition: merge] [Allow leading pipe in matches!() patterns.](https://github.com/rust-lang/rust/pull/85272)
* [disposition: close] [Add expr202x macro pattern](https://github.com/rust-lang/rust/pull/84364)
* [disposition: merge] [Remove P: Unpin bound on impl Future for Pin](https://github.com/rust-lang/rust/pull/81363)
* [disposition: merge] [Stabilize core::task::if_ready!](https://github.com/rust-lang/rust/pull/81050)
* [disposition: merge] [Tracking Issue for IntoInnerError::into_parts etc. (io_into_inner_error_parts)](https://github.com/rust-lang/rust/issues/79704)
* [disposition: close] [Implement RFC 2500 Needle API (Part 1)](https://github.com/rust-lang/rust/pull/76901)

### New RFCs

* [RFC: map_or_default in Option and Result](https://github.com/rust-lang/rfcs/pull/3148)
* [Cargo feature migrations](https://github.com/rust-lang/rfcs/pull/3146)

## Upcoming Events

### Online

* [July 14, 2021, Malaysia - Rust Meetup July 2021 - Golang Malaysia, feat Rustlang, Erlang, Haskelllang and `.*-?(lang|script)\`](https://docs.google.com/forms/d/e/1FAIpQLSdoVbexvU3TZox1D9yLKPUggeTuih7TEDR6eaFQGTEgJtXZ5g/viewform)
* [July 14, 2021, Dublin, IE - Rust Dublin July Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/278698763/)
* [July 20, 2021, Washington, DC, US - Mid-month Rustful - Rust DC](https://www.meetup.com/RustDC/events/vdhxgsycckbbc/)
* [July 21, 2021, Vancouver, BC, CA - Rust Adoption at Huawei - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/zkqvjsycckbcc/)
* [July 22, 2021, Tokyo, JP - Rust LT Online#4 - Rust JP](https://www.youtube.com/watch?v=oK0iJz7XF3Y)
* [July 22, 2021, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/)
* [July 27, 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwrycckbkc/)

### North America

* [July 14, 2021, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgrycckbsb/)
* [July 27, 2021, Chicago, IL, US - Rust in production at Tempus - Chicago Rust Meetup](https://www.meetup.com/Chicago-Rust-Meetup/events/279131036)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**PolarFox Network**
* [Senior Rust Engineer (Remote)](https://jro-ventures.breezy.hr/p/0c1d3630d39d)

**CNRS**
* [Rust Software Engineer in AI research applied to Robotics (Toulouse, France)](https://emploi.cnrs.fr/Offres/CDD/UPR8001-ARTBIT-004/Default.aspx?lang=EN)

**The Mobility House GmbH**
* [Senior Software Engineer - Rust m/f/d (Remote / Germany)](https://germantechjobs.de/jobs/The-Mobility-House-GmbH-Senior-Software-Engineer-mfd)

**Immunant**
* [Systems Programmer/Rustacean (Optionally Remote)](https://immunant.com/jobs/)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Beginning Rust: Uh why does the compiler stop me from doing things this is horrible
>
> Advanced Rust: Ugh why doesn't the compiler stop me from doing things this is horrible

– [qDot on twitter](https://twitter.com/qDot/status/1412536312150716416)

Thanks to [Nixon Enraght-Moony](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1074) for the self-suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/k5nsab/this_week_in_rust_367/)</small>
