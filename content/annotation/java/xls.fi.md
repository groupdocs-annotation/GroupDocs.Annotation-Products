---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java XLS Annotation API Annotate in C#"
head_description: "Java-sovellusliittymä suosittujen huomautustyyppien luomiseen ja merkitsemiseen XLS-tiedostoista, kuvista, piirustuksista ja asiakirjatiedostomuodoista."

############################# Header ############################
title: "Merkitse XLS Javasta"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Lataa ilmainen kokeiluversio"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Tietoja GroupDocs.Annotation for Java API:sta"
    content: |
        GroupDocs.Annotation for Java API on kirjasto, jonka avulla voit lisätä huomautuksia PDF-, Word- ja muihin asiakirjoihin Macissa, Windowsissa tai Ubuntussa. [GroupDocs.Annotation for Java](/annotation/java) on natiivi Java-sovellusliittymä merkintöjen hallintaan, ja siinä on kattava tuki merkintöjen luomiseen, lisäämiseen, muokkaamiseen, poistamiseen, poimimiseen ja vientiin kuvista ja useista muista asiakirjoista. Täydellinen luettelo tuetuista asiakirjamuodoista löytyy tällä [sivulla](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Tämän kirjaston avulla voit työskennellä XLS-asiakirjan lisäksi myös monien muiden asiakirjojen kanssa, kuten Word, Excel, PowerPoint, Outlook-sähköpostit, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ja monet muut.
        GroupDocs.Annotation for Java API:n avulla voit luoda ja lisätä uusia muistiinpanoja, muokata huomautuksia, poimia kommentteja, merkintöjä ja poistaa niitä asiakirjoista. Kirjasto tukee 13 erilaista merkintätyyppiä, mukaan lukien teksti, polyline, alue, alleviivaus, piste, vesileima, nuoli, ellipsi, tekstin vaihto, etäisyys, tekstikenttä, resurssien muokkaus PDF-, HTML-, Microsoft Word -asiakirjoissa, laskentataulukoissa, kaavioissa, esityksissä, piirustuksia, kuvia ja monia muita tiedostomuotoja.
        Esimerkki (katso alla) havainnollistaa työskentelyä asiakirjan XLS kanssa. Tässä esimerkissä voit nähdä GroupDocsin työskentelyn päävaiheet. Huomautus: Määritä lisenssi, avaa dokumentti, jota haluat käsitellä, ja luo huomautus, tietoobjektien lisääminen merkintöjen ominaisuuksien määrittämiseksi tarpeidesi mukaan ja tuloksen tallentaminen haluttuun paikkaan. Voit myös tutustua tarkemmin tuettuihin ominaisuuksiin github-sivullamme [sivulla](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) tai tuotteessamme [dokumentaatiossa](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Ohjeet merkintöjen lisäämiseen Java-tiedostoon XLS"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) tekee Java-kehittäjien helpoksi lisätä erilaisia ​​huomautustyyppejä XLS-tiedostoihin missä tahansa Java-pohjaisessa sovelluksessa toteuttamalla muutaman helpon vaiheen.
        *   Luo vastausobjekteja kommentilla ja päivämäärällä.
        *   Luo AreaAnnotation-objekti, aseta alueasetukset ja lisää vastauksia.
        *   Luo Annotator-objekti ja lisää alueen huomautus.
        *   Tallenna tulostiedosto.
    title_right: "Laitteistovaatimukset"
    content_right: |
        GroupDocs.Annotation Java-sovellusliittymille tuetaan kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.
        *   Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        *   Kehitysympäristö: NetBeans, Intellij IDEA, Eclipse jne
        *   Java Runtime Environment: Java 7 (1.7) tai uudempi
        *   Hanki GroupDocs.Annotation for Java uusin versio [GroupDocs Artifact Repositorysta](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Huomautuksen esikatselu ja koodinäyte
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Create an instance of Reply class and add comments
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("This is area annotation");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Add annotation
        annotator.add(area);
        
        // Save to file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Ohjeet merkintöjen poistamiseen Java-tiedostosta XLS"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Helpottaa Java-kehittäjien merkintöjen tietojen poistamista XLS-tiedostoista missä tahansa Java-pohjaisessa sovelluksessa toteuttamalla muutaman helpon vaiheen.
        *   Luo vastausobjekteja kommentilla ja päivämäärällä.
        *   Luo SaveOptions-objekti ja aseta AnnotationTypes = AnnotationType.None.
        *   Kutsu tallennusmenetelmää tuloksena olevalla asiakirjapolulla tai -virralla ja SaveOptions-objektilla.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```java
        // Create an instance of Annotator class 
        Annotator annotator = new Annotator("C://input.bmp");

        // Remove annotation by set type None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Save annotation to output file
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Ohjeet merkintöjen muokkaamiseen Javassa tiedostosta XLS"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) helpottaa Java-kehittäjien merkintöjen ominaisuuksien päivittämistä XLS-tiedostoista missä tahansa Java-pohjaisessa sovelluksessa toteuttamalla muutaman helpon vaiheen.
        *   Instantoi Annotator-objekti syöteasiakirjan polulla tai virralla instantoiduilla LoadOptions-toiminnoilla, kun ImportAnnotations = true.
        *   Luo jokin AnnotationBase-toteutus ja aseta olemassa olevan merkinnän tunnus (jos merkintää tällä tunnuksella ei löydy, mitään ei muuteta) tai merkintöjen polkuluettelo (kaikki olemassa olevat merkinnät poistetaan).
        *   Kutsu Annotator-objektin päivitysmenetelmä hyväksytyillä huomautuksilla.
        *   Kutsu tallennusmenetelmää tuloksena olevalla asiakirjapolulla tai -virralla ja SaveOptions-objektilla.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Create an instance of Reply class for first example and add comments
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Create an instance of Reply class for update first example
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Update and save annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Ohjeet merkintöjen purkamiseen Java-tiedostosta XLS"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Helpottaa Java-kehittäjien merkintöjen tekemistä asiakirjoihin ja merkintätietojen poimia XLS-tiedostoista missä tahansa Java-pohjaisessa sovelluksessa muutaman helpon vaiheen avulla.
        *   Luo vastausobjekteja kommentilla ja päivämäärällä.
        *   Luo LoadOptions-objekti ja kutsu SetImportAnnotations tosi-argumentilla.
        *   Määrittele muuttuja tyypillä List.
        *   Kutsu get-metodi ja palauta tulos yllä olevaan muuttujaan.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```java
        // For using this example input file ("annotated.bmp") must be with annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Create an instance of Annotator class and get annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Live-esittelyt asiakirjojen ja kuvien huomautusten lisäämiseen, poistamiseen, muokkaamiseen ja poimimiseen"
    content: |
        Lisää, poista, muokkaa ja pura merkintöjä tiedostoon XLS heti käymällä [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) -sivustolla.
Live-demolla on seuraavat edut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xls"
          title: "Tietoja tiedostomuodosta XLS"
          content: |
            XLS-laajennuksella varustetut tiedostot edustavat Excelin binaaritiedostomuotoa. Tällaisia ​​tiedostoja voidaan luoda Microsoft Excelillä sekä muilla vastaavilla taulukkolaskentaohjelmilla, kuten OpenOffice Calc tai Apple Numbers. Excelin tallentamaa tiedostoa kutsutaan työkirjaksi, jossa jokaisessa työkirjassa voi olla yksi tai useampi laskentataulukko. Tiedot tallennetaan ja näytetään käyttäjille taulukkomuodossa laskentataulukossa, ja ne voivat sisältää numeerisia arvoja, tekstidataa, kaavoja, ulkoisia tietoyhteyksiä, kuvia ja kaavioita. Microsoft Excelin kaltaisten sovellusten avulla voit viedä työkirjan tietoja useisiin eri muotoihin, mukaan lukien PDF, CSV, XLSX, TXT, HTML, XPS ja monet muut. XLS-tiedostomuoto korvattiin avoimemmalla ja jäsennellymmällä XLSX-muodolla Microsoft Excel 2007:n julkaisun myötä. Uusimmat versiot tukevat edelleen XLS-tiedostojen luomista ja lukemista, vaikka XLSX onkin nyt ensimmäinen käyttövaihtoehto.

          link: "https://docs.fileformat.com/image/xls/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Työskentely muiden suosittujen asiakirjamuotojen kanssa"
    content: |
        Päivitä merkintöjen ominaisuudet joistakin suosituista tiedostomuodoista alla kuvatulla tavalla.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/java/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/java/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/java/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/java/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/java/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/java/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/java/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/java/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/java/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/java/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/java/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/java/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/java/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/java/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/java/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/java/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/java/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/java/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/java/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/java/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/java/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/java/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/java/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/java/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/java/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/java/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/java/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/java/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/java/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/java/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/java/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/java/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/java/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/java/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/java/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---