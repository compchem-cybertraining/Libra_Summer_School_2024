---
layout: workshop
venue: "University at Buffalo, SUNY"   # brief name of host site without address (e.g., "Euphoric State University")
address: "University at Buffalo, SUNY, North Campus, Natural Sciences Complex"   # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "United States"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
latitude: "43.002890"     # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-78.788780"    # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "January 9-15, 2022"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "09:00 am - 5:00 pm EDT"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2022-01-09      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2022-01-15        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Alexey Akimov"] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: ["Mohammad Shakiba" ] # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["alexeyak@buffalo.edu"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes:   # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
googleform: https://forms.gle/5PW6EKwAPHEPy5b6A
carpentry: "sc"
---


{% comment %}
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
{% endcomment %}


# Libra Winter School on Excited States and Nonadiabatic Dynamics in Materials 2022

### About the Winter School

The Libra Winter School aims to provide training to graduate students, postdocs, researchers, and educators working in
 a broader field of nonadiabatic and excited-state dynamics as well as in computational material sciences. The workshop 
will provide conceptual and practical hands-on training in a range of methods for modeling excited state and nonadiabatic 
dynamics in abstract models and atomistic materials. Nearly all activities will leverage and showcase the capabilities of 
the Libra code developed by the instructors group. They will learn to install and use the Libra package for building 
atomistic models, computing excited states of molecular and periodic systems, as well as pre- and post-processing operations, 
and data analysis. The participants will also learn to use several popular electronic structure packages such as CP2K, 
Quantum Espresso, and DFTB+/xTB and how these packages could be used with Libra to conduct atomistic modeling of the excited 
states and nonadiabatic dynamics in realistic materials.

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
- TD-DFT
- algorithms and methods
- software, programming, Python

### Hands-on with software 
 
The school will leverage the [OnDemand](https://ondemand.ccr.buffalo.edu) gateway at the University at Buffalo and will 
focus on the following codes:

- [Libra](https://github.com/Quantum-Dynamics-Hub/libra-code/tree/devel) - **primarily**
- [CP2K](https://www.cp2k.org/)
- [DFTB+ and xTB](https://dftbplus.org)
- [Quantum Espresso](https://www.quantum-espresso.org/)


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

### Schedule

{% include base_path.html %}

The details may vary and the order of topics may be changed, the topics may be omitted or added. Please check for the updates. 

  <table class="table table-striped">
  
  <tr>
    <td class="col-md-3"><strong>Date</strong></td>
    <td class="col-md-9"><strong>Topics</strong></td> 
  </tr>

  <tr>
    <td class="col-md-3">January 9, 2022, Sunday</td>
    <td class="col-md-9">
      <ul>        
        <li>Arrivals and Welcome dinner.</li>
      </ul>
    </td> 
  </tr>
  
  <tr>
    <td class="col-md-3">January 10, 2022 (Day 1), Monday</td>
    <td class="col-md-9">
      <ul>        
        <li>Opening. Intro to Jupyter and Python. </li>
        <li>Introduction to Adiabatic and Nonadiabatic molecular dynamics.</li>
        <li>Libra installation and testing examples.</li>
        <li>Classical MD with the force fields in Libra. Exploring PESs.</li>
      </ul>
    </td> 
  </tr>

  <tr>
    <td class="col-md-3">January 11, 2022 (Day 2), Tuesday</td>
    <td class="col-md-7">
      <ul>
        <li>General overview of the Libra code.</li> 
        <li>TSH and Ehrenfest dynamics: model Hamiltonians in Libra.</li>
        <li>Hierarchy of equations of motion (HEOM) calculations with Libra. </li>
        <li>Wavepacket/DVR calculations with  Libra. </li>
      </ul>
    </td>
  </tr>

  <tr>
    <td class="col-md-3">January 12, 2022 (Day 3), Wednesday</td>
    <td class="col-md-9">
      <ul>
        <li>Electronic structure theory overview.</li>
        <li>Libra' semiempirics and built-in integrals.</li>
        <li>Hands on with Quantum Espresso.</li>
        <li>Hands on with DFTB+.</li>
        <li>Hands on with CP2k/xTB.</li>
      </ul>
    </td>
  </tr>

  <tr>
    <td class="col-md-3">January 13, 2022 (Day 4), Thursday</td>
    <td class="col-md-9">
      <ul>
        <li>Atomistic simulations of NA-MD in materials, using Libra/DFTB+, Libra/cp2k, and Libra/QE interfaces.</li>
      </ul>
    </td>
  </tr>

  <tr>
    <td class="col-md-3">January 14, 2022 (Day 5), Friday</td>
    <td class="col-md-9">
      <ul>
        <li>Continued: Atomistic simulations of NA-MD in materials, using Libra/DFTB+, Libra/cp2k, and Libra/QE interfaces.</li>
        <li>Additional capabilities of Libra: introduction to neural networks/machine learning.</li>
        <li>Closing. Exploring Buffalo.</li>
      </ul>
    </td>
  </tr>
  
  <tr>
    <td class="col-md-3">January 15, 2022, Saturday</td>
    <td class="col-md-9">
      <ul>
        <li>Exploring Buffalo/Departure.</li>
      </ul>
    </td>
  </tr>

  </table>


### Instructor and co-instructors

 * [Dr. Alexey Akimov](https://akimovlab.github.io/) - University at Buffalo, USA
 * [Mr. Mohammad Shakiba]() - University at Buffalo, USA

### Administrative support

 * [UB CCR](http://www.buffalo.edu/ccr.html)  - UB Center for Computational Research (CCR), UB VPN, Open OnDemand, HPC accounts, etc.
 

## Participation

### Who can apply

This winter school is primarily for graduate students working in computational modeling of excited states and nonadiabatic 
dynamics, both in abstract and atomistic applications/problems. Senior undergraduate students with relevant experience and 
training are also welcome.

The school aims to help researchers/students working either in methodology development for nonadiabatic or quantum-classical 
dynamics and in applied studies of various types of solar energy materials (photovoltaics, photocatalytics, etc.).

Postdocs and researchers wishing to acquire practical experience with new simulation tools and expand their knowledge 
in the areas of excited states and nonadiabatic dynamics are also welcome to participate.

There is no restriction for the international applicants to participate, but keep in mind that the international travel
expenses may not be covered in full. 


### How to apply to the school

1. Read this page carefully
2. Prepare your application package (you will need it in the next steps)

   2.1. your CV (including graduate or undergraduate GPA)

   2.2. a statement of purpose PDF should describe in no more than 2 pages:

   * your current/ongoing research projects and interests; 

   * if and how you plan to use the Libra software in your research;
         
   2.3. request your advisor to submit a letter of recommendation for you to the following email: "alexeyak AT buffalo DOT edu", 
   please replace "AT" and "DOT" with the corresponding characters

3. Complete the <a href="https://forms.gle/5PW6EKwAPHEPy5b6A" target="_blank" rel="nofollow">**Registration form**</a>


### Important dates
   * Workshop application materials are due 5 pm EST, Dec. 3, 2021
   * Applicants are notified of their admission by 5 pm EST, Dec. 10, 2021
   * Workshop starts: 9 am EST, January 10, 2022  (welcome dinner the evening before)
   * Workshop ends: 5 pm EST, January 14, 2022 (departure next day)


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
