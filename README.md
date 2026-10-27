# CV Website – Alex Ferrer

> [!NOTE]
> All the information is made up

A single-page static website that presents my Curriculum Vitae and a small portfolio of projects.

- **Live site:** `https://josepbarnada.github.io/MIU---CV/`
- **Figma design:** `<https://www.figma.com/design/GTVM1nA15LHDkdZZrfcqJx/Untitled?node-id=0-1&t=pVqH7W72e1ZNFCHU-1>`

---

## 1. Project analysis

### 1.1 User profile (persona)

**Marta Soler, 38, Talent Acquisition Specialist at a software company in Barcelona**

|                    |                                                                                                  |
| ------------------ | ------------------------------------------------------------------------------------------------ |
| **Role**           | Screens junior developer applications for a mid-sized tech company                               |
| **Context**        | Reviews 30–50 candidates per vacancy, often on a laptop between meetings, sometimes on her phone |
| **Time per CV**    | 20–30 seconds on a first pass                                                                    |
| **Tech knowledge** | Medium: knows the names of technologies but not the details                                      |

**Goals**

- Quickly see who the candidate is, what they study or do, and whether they match the profile.
- Find the key skills (languages, frameworks) at a glance.
- Check real experience and see proof of work (projects, GitHub).
- Contact the candidate easily.

**Frustrations**

- Long, dense CVs with no visual hierarchy.
- Missing or hidden contact details.
- Portfolios that are broken, slow or impossible to navigate.

**What she expects to find:** a clean one-page CV with a clear name and title, a short bio, skills, a timeline of experience and education, languages, and links to projects and professional profiles.

_Secondary user:_ a fellow developer or professor who wants to look at the code of my projects and judge the quality of my work.

### 1.2 Information architecture

The site is a single page whose content is ordered by what a recruiter wants to know first, following the "top-to-bottom, most important first" principle and an F-shaped reading pattern.

1. **Personal information (top banner).** Photo, name, professional title ("Computer Science Student") and a short bio. This answers "who is this person?" within the first seconds, and the photo adds a human touch.
1. **Two-column middle section.** The page is divided into a narrow sidebar and a wider main column.
   - **Left sidebar, "useful info":** Contact (email, GitHub, LinkedIn, location), Skills and Languages. These are short, scannable pieces of information that a recruiter wants to check quickly or copy, so they stay visible next to the main content.
   - **Right column, "experience":** Work Experience and Education, each displayed as a chronological timeline, most recent first. Every entry has a date, a title, an organisation and, where relevant, bullet points with what I did.
1. **Projects (bottom, full width).** Each project has a year, a name linking to the project and a one-line description. Projects come last because they are supporting evidence that backs up the skills and experience read above.

Grouping the content in these blocks keeps the page short enough to scan without much scrolling, and using the same timeline component (date + marker + content) for experience, education and projects gives the page a consistent structure that is easy to learn after the first entry.

### 1.3 Visual design

**Layout.** I used a simple grid-based layout with a header, a sidebar plus main column, and a full-width footer section for projects. White space between sections separates the content without needing heavy borders. On smaller screens the columns are meant to stack vertically (sidebar first, then experience and projects) so the page stays readable on mobile.

**Colour palette.** The design uses a neutral base (white or very light grey background with dark grey text) for readability and professionalism, plus **one accent colour** that is applied through the `.accent` class. The accent is used for the professional title and the skills, and for the timeline markers, so the eye is guided to the most important elements. Using a single accent avoids visual noise and keeps the CV serious but modern. Text and background colours keep a contrast ratio above the WCAG AA minimum (4.5:1).

**Typography.** I chose a clean sans-serif font family, because it is legible on screens at small sizes and fits a technical profile. Hierarchy is created through size and weight rather than many different fonts: `h1` for the name, `h2` for section titles, `h3` for job, degree and project titles, and a lighter, smaller grey style (`.description`) for secondary details such as dates and organisations.

**Components.** The timeline (a date, a small circular marker and the content) is the central visual element. It communicates chronology at a glance and is reused for experience, education and projects. Skills are displayed as short tags in the accent colour, which makes them easy to scan. The profile picture is shown at a fixed 150×150 size, which gives the header a personal touch.

**Inspiration.** I looked at minimalist developer CV and portfolio templates (for example on Behance, Dribbble and GitHub Pages portfolios) and at the "Europass"-style CV structure, adapting them to a more modern, lighter look.

**Responsiveness.** The layout uses flexible units and media queries so it works on desktop first and adapts to tablet and mobile screens.
