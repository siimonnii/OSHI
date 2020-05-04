Representative metadata for OSH
=

As documentation is technology-specific, reasonable metadata may be as well. 
This first draft assumes that metadata must be technology-specific in order to give a meaningful representation
and hence enable meaningful connections between OSH modules.

# OSH Module (OKH-MOD)

**Intro:**

- = assembly of components (and subassemblies) with clear input, output and interfaces 
  - (and thus can be used independently from the rest of the original machine as far as required inputs and interfaces are respected);
- metadata shall represent functionality and "position inside the OSH ecosystem" (→ BoM = link to other modules)

**Metadata:**

- name or working title
- version
    - of hardware design
    - of documentation
- link to [OKH-ASM](#osh-assembly-okh-asm) (manifest file for assemblies)
- link to LICENSE.md
- link to README.md
- link to CONTRIBUTING.md
- functional description (e.g. what functions it is supposed to deliver, what is the problem it solves, for whom etc.)
    - → use guidelines for naming convention e.g. [as for inventions](https://www.wipo.int/export/sites/www/standards/en/pdf/03-15-01.pdf)
- applying technology-specific documentation criteria ([TsDC-IDs](https://gitlab.com/OSEGermany/oh-tsdc/-/blob/master/TsDC-DB-print.md))
- link to [standardised BoM](#standardised-bom)
- (link to) functional metadata ← _very_ technology-specific! not to be standardised here
  - dimensions
  - material
  - weight
  - RPM
  - …

## standardised BoM

= for documentation purposes; easy to read, crawl and use (maybe call **meta-BoM**?)

| Pos. | Name         | Units | Type           | Reference                                 |
|------|--------------|-------|----------------|-------------------------------------------|
| 1    | casing       | 2     | OSH Component  | link to [OKH-COM](#osh-component-okh-com) |
| 2    | screw        | 4     | standard part  | standard designation                      |
| 3    | gear box     | 1     | OSH Module     | link to [OKH-MOD](#osh-module-okh-mod)    |
| 4    | Raspberry Pi | 1     | purchased part | unambiguous reference (not standardised)  |

## OSH assembly (OKH-ASM)

**Intro:**

- = assembly of components
- metadata shall enable reproduction, operation and maintenance

**Metadata:**

- name or working title
- version
    - of hardware design
    - of documentation

## OSH component (OKH-COM)

**Intro:**

- = undevided, self-designed piece of hardware to be manufactured
- metadata shall enable reproduction, operation and maintenance

**Metadata:**

- name or working title
- version
    - of hardware design
    - of documentation
- authors
- license
- link to design files
    - 3D model
        - source → script gets file format
        - export (STD)
    - 2D drawing
        - source → script gets file format
        - export (PDF)