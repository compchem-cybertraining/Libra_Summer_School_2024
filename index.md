---
layout: workshop
venue: "University at Buffalo, SUNY"   # brief name of host site without address (e.g., "Euphoric State University")
address: "University at Buffalo, SUNY, North Campus, Natural Sciences Complex"   # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "United States"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
latitude: "43.002890"     # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-78.788780"    # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "July 7-13, 2024"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "09:00 am - 5:00 pm EDT"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2024-07-07      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2022-07-13        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Alexey Akimov"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["Mohammad Shakiba", "Daeho Han" ] # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["alexeyak@buffalo.edu"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes:   # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
googleform: https://forms.gle/5PW6EKwAPHEPy5b6A
carpentry: "sc"
---


{% comment %}
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
{% endcomment %}


# Libra Summer School on Excited States and Nonadiabatic Dynamics in Materials 2024

### About this Summer School

This Libra Summer School will provide training to the graduate students, postdocs, and researchers on applying 
mixed quantum-classical methods for nonadiabatic and excited-state dynamics available in the Libra software. 
The key theoretical and conceptual grounds of such simulations and practical details on the implementation and 
execution of these methods will be covered. The participants will go through a series of practical hands-on 
exercises to experience a range of methods and computational workflows available in the Libra software. 
Modeling of excited state and nonadiabatic dynamics will be conducted for the abstract Hamiltonians and atomistic 
models of materials. Some of the latest capabilities of Libra will be highlighted, such as using machine learning 
approaches for nonadiabatic dynamics in materials, using exact factorization and Gaussian-wavepacket-based 
trajectory surface hopping methods, or applying a broad range of decoherence corrections in various situations. 
The participants will improve their knowledge of some electronic structure packages interfaced with Libra code, 
particularly the CP2K package.


### Keywords and topics

- nonadiabatic dynamics
- excited states
- solar energy materials 
- condensed matter
- nanoparticles
- quantum dynamics
- quantum-classical methods
- charge transfer
- excitation energy transfer
- trajectory surface hopping
- machine learning
- trajectory surface hopping
- exact factorization
- decoherence corrections
- TD-DFT
- algorithms and methods
- software, programming, Python

### Hands-on with software 
 
The school will leverage the [OnDemand](https://ondemand.ccr.buffalo.edu) gateway at the University at Buffalo and will 
focus on the following codes:

- [Libra](https://github.com/Quantum-Dynamics-Hub/libra-code/tree/devel) - **primarily**
- [CP2K](https://www.cp2k.org/)
- [DFTB+ and xTB](https://dftbplus.org)


## Logistics

{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% if page.latitude and page.longitude %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latitude}}&mlon={{page.longitude}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latitude}},{{page.longitude}}">Google Maps</a>.
</p>
{% endif %}

{% comment %}
CONTACT EMAIL ADDRESS
Display the contact email address set in the configuration file.
{% endcomment %}
<p id="contact">
  <strong>Contact</strong>:
  Please email
  {% if page.email %}
  {% for email in page.email %}
  {% if forloop.last and page.email.size > 1 %}
  or
  {% else %}
  {% unless forloop.first %}
  ,
  {% endunless %}
  {% endif %}
  <a href='mailto:{{email}}'>{{email}}</a>
  {% endfor %}
  {% else %}
  to-be-announced
  {% endif %}
  for more information.
</p>


### Instructor and co-instructors

 * [Dr. Alexey Akimov](https://akimovlab.github.io/) - University at Buffalo, USA
 * [Dr. Daeho Han]() - University at Buffalo, USA
 * [Mr. Mohammad Shakiba]() - University at Buffalo, USA

### Administrative support

 * [UB CCR](http://www.buffalo.edu/ccr.html)  - UB Center for Computational Research (CCR), UB VPN, Open OnDemand, HPC accounts, etc.
 

## Participation

### Who can apply

This summer school is primarily for graduate students/postdocs/researchers working in computational modeling of excited states and nonadiabatic 
dynamics, either abstract or atomistic applications/problems. Exceptional senior undergraduate students with relevant experience and 
training may be considered.

Due to the limited number of slots, only one participant per research group is allowed.

There is no restriction for the international applicants to participate, but keep in mind that the international travel
expenses may not be covered in full. 


### How to apply to the school

1. Read this page carefully
2. Prepare your application package (you will need it in the next steps)

   2.1. your CV (including graduate or undergraduate GPA)

   2.2. a statement of purpose PDF should describe in no more than 2 pages:

   * your current/ongoing research projects and interests; 

   * your prior experience with Libra package or a plan on how you envision to leverage Libra software in your research;
         
   2.3. request your advisor to submit a letter of recommendation for you to the following email: "alexeyak AT buffalo DOT edu", 
   please replace "AT" and "DOT" with the corresponding characters

3. Complete the <a href="https://forms.gle/5PW6EKwAPHEPy5b6A" target="_blank" rel="nofollow">**Registration form**</a>


### Important dates
   * Workshop application materials are due 5 pm EST, Dec. 3, 2021
   * Applicants are notified on their admission by 5 pm EST, Dec. 10, 2021
   * Workshop starts: 9 am EST, July 8, 2024  (welcome dinner on the evening before)
   * Workshop ends: 5 pm EST, July 12, 2024 (departure next day)


### Selection and restrictions

The anticipated class size is about 10 people, so the selection is competitive. In particular, this 
means that we may limit the selection of applicants from the same research group or institution. 

The applicants will be selected based on the strength of their statement of purpose, as well as the 
adequate support of their supervisors and their level of fundamental preparation. The lack of training 
in specialized methods and software is not a problem. What is more important is how ready the applicant 
is to absorb new knowledge, how efficiently they can operate during the workshop, and how critical 
the use of the methods/tools covered in the workshop may be for your future research or career.


### Successful applicants

The successful applicants will be provided with stipends toward covering their logging, meal, and travel expenses.

There is a limit on the travel expenses that we can reimburse, so any extra costs are up for the participants to cover. 
This is especially the case for any potential international participants. 


### Acknowledgement

This workshop is made possible by the NSF-CSSI program. Thank you!


{% include links.md %}
