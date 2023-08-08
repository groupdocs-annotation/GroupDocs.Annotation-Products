---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net ODS Annotation API Annotate in C#"
head_description: "Net API პოპულარული ანოტაციის ტიპების შესაქმნელად და ანოტაციისთვის ODS-დან, სურათებიდან, ნახატებიდან და დოკუმენტის ფაილის ფორმატებიდან."

############################# Header ############################
title: "ანოტაცია ODS Net-დან"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "ჩამოტვირთეთ უფასო საცდელი"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Annotation-ის შესახებ Net API-სთვის"
    content: |
        GroupDocs.Annotation for Net API არის ბიბლიოთეკა, რომელიც საშუალებას გაძლევთ დაამატოთ ანოტაციები PDF, Word და სხვა დოკუმენტებში Mac, Windows ან Ubuntu-ზე. [GroupDocs.Annotation for Net](/annotation/net) არის მშობლიური Net API ანოტაციების მართვისთვის ყოვლისმომცველი მხარდაჭერით სურათებიდან ან სხვა დოკუმენტებიდან ანოტაციების შექმნის, დამატების, რედაქტირების, წაშლის, ამოღებისა და ექსპორტისთვის. მხარდაჭერილი დოკუმენტის ფორმატების სრული სია, რომელიც შეგიძლიათ იხილოთ ამ [გვერდზე] (https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        ეს ბიბლიოთეკა საშუალებას გაძლევთ იმუშაოთ არა მხოლოდ ODS დოკუმენტთან, არამედ მრავალი სხვა ტიპის დოკუმენტთან, როგორიცაა Word, Excel, PowerPoint, Outlook ელფოსტა, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad და მრავალი სხვა.
        GroupDocs.Annotation Net API-სთვის საშუალებას გაძლევთ შექმნათ და დაამატოთ ახალი შენიშვნები, დაარედაქტიროთ ანოტაციები, ამოიღოთ კომენტარები, ანოტაციები და წაშალოთ ისინი დოკუმენტებიდან. ბიბლიოთეკა მხარს უჭერს 13 სხვადასხვა ტიპის ანოტაციას, მათ შორის ტექსტს, პოლიხაზს, ფართობს, ხაზს, წერტილს, ჭვირნიშანს, ისარს, ელიფსს, ტექსტის ჩანაცვლებას, მანძილს, ტექსტის ველს, რესურსების რედაქციას PDF, HTML, Microsoft Word დოკუმენტებში, ცხრილებში, დიაგრამებში, პრეზენტაციებში, ნახატები, სურათები და მრავალი სხვა ფაილის ფორმატი.
        მაგალითი (იხილეთ ქვემოთ) ასახავს ODS დოკუმენტთან მუშაობას, ამ მაგალითში შეგიძლიათ იხილოთ GroupDocs-თან მუშაობის ძირითადი ნაბიჯები. ანოტაცია: დააყენეთ ლიცენზია, გახსენით დოკუმენტი, რომელთანაც გსურთ მუშაობა, შექმნათ ანოტაცია, მონაცემთა ობიექტების დამატება ანოტაციის თვისებების დასაყენებლად თქვენი მოთხოვნების შესაბამისად და შედეგის შესანახად საჭირო ადგილას. ასევე შეგიძლიათ უფრო დეტალურად გაეცნოთ მხარდაჭერილ ფუნქციებს ჩვენს github-ზე [გვერდზე](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), ან ჩვენს პროდუქტში [დოკუმენტაცია](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "ნაბიჯები ანოტაციების დასამატებლად ODS Net-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net-ის დეველოპერებს უადვილებს ანოტაციის სხვადასხვა ტიპების დამატებას ODS ფაილზე ნებისმიერი Net-ზე დაფუძნებული აპლიკაციის ფარგლებში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   შექმენით პასუხის ობიექტები კომენტარებით და თარიღით.
        *   შექმენით AreaAnnotation ობიექტი, დააყენეთ არეალის პარამეტრები და დაამატეთ პასუხები.
        *   შექმენით Annotator ობიექტი და დაამატეთ არეალის ანოტაცია.
        *   შეინახეთ გამომავალი ფაილი.
    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Annotation Net API-ებისთვის მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.
        *   ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        *   განვითარების გარემო: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   ჩამოტვირთეთ GroupDocs.Annotation-ის უახლესი ვერსია .NET-ისთვის [NuGet]-დან (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: ანოტაციის გადახედვა და კოდის ნიმუში
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
        using (Annotator annotator = new Annotator("input.bmp"))
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "This is text field annotation",
                Opacity = 0.7,
                PageNumber = 0,
                PenStyle = PenStyle.Dot,
                PenWidth = 3,
                FontFamily = "Arial",
                TextHorizontalAlignment = HorizontalAlignment.Center,
                Replies = new List
                {
                    new Reply
                    {
                        Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "ნაბიჯები ანოტაციების წასაშლელად ODS-დან Net-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net-ის დეველოპერებს უადვილებს ანოტაციის დეტალების წაშლას ODS ფაილებიდან ნებისმიერი Net-ზე დაფუძნებული აპლიკაციიდან რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   შექმენით პასუხის ობიექტები კომენტარებით და თარიღით.
        *   შექმენით SaveOptions ობიექტი და დააყენეთ AnnotationTypes = AnnotationType.None.
        *   ზარის შენახვის მეთოდის შედეგი დოკუმენტის გზა ან ნაკადი და SaveOptions ობიექტი.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "ნაბიჯები ანოტაციების რედაქტირებისთვის ODS-დან Net-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) უადვილებს Net-ის დეველოპერებს განაახლონ სხვადასხვა ანოტაციის თვისებები ODS ფაილებიდან ნებისმიერი Net-ზე დაფუძნებული აპლიკაციის ფარგლებში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   Instantiate Annotator ობიექტის შეყვანის დოკუმენტის გზა ან ნაკადი instantiated LoadOptions ერთად ImportAnnotations = true.
        *   შექმენით AnnotationBase იმპლემენტაცია და დააყენეთ არსებული ანოტაციის ID (თუ ანოტაცია ამ Id-ით ვერ მოიძებნა, არაფერი შეიცვლება) ან ანოტაციების ბილიკის სია (ყველა არსებული ანოტაცია წაიშლება).
        *   Annotator ობიექტის ზარის განახლების მეთოდი გადაცემული ანოტაციებით.
        *   ზარის შენახვის მეთოდის შედეგი დოკუმენტის გზა ან ნაკადი და SaveOptions ობიექტი.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```cs
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Updated first comment",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Updated second comment",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "ნაბიჯები ანოტაციების ამოსაღებად ODS-დან Net-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net-ის დეველოპერებს უადვილებს დოკუმენტების ანოტაციას და ანოტაციის ინფორმაციის ამოღებას ODS ფაილებიდან ნებისმიერი Net-ზე დაფუძნებული აპლიკაციის ფარგლებში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   შექმენით პასუხის ობიექტები კომენტარებით და თარიღით.
        *   Instantate LoadOptions ობიექტი და გამოიძახეთ SetImportAnnotations ჭეშმარიტი არგუმენტით.
        *   განსაზღვრეთ ცვლადი სია ტიპის მიხედვით.
        *   გამოიძახეთ get მეთოდი და დააბრუნეთ შედეგი ზემოთ ცვლადში.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```cs
        // for using this example input file ("annotated.bmp") must be with annotations
        using (Annotator annotator = new Annotator("annotated.bmp"))
        {
            List annotations = annotator.Get();
            XmlSerializer formatter = new XmlSerializer(typeof(List));
            using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
                fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "ცოცხალი დემოები დოკუმენტებსა და სურათებზე ანოტაციების დასამატებლად, ამოსაღებად, რედაქტირებისთვის"
    content: |
        დაამატეთ, წაშალეთ, დაარედაქტირეთ და ამოიღეთ ანოტაციები ODS ფაილში ახლავე, ეწვიეთ [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) ვებსაიტს. ცოცხალი დემოს აქვს შემდეგი უპირატესობები

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ods"
          title: "ODS ფაილის ფორმატის შესახებ"
          content: |
            ფაილები ODS გაფართოებით არის OpenDocument Spreadsheet დოკუმენტის ფორმატი, რომელიც რედაქტირებადია მომხმარებლის მიერ. მონაცემები ინახება ODF ფაილში რიგებად და სვეტებად. ეს არის XML-ზე დაფუძნებული ფორმატი და არის ღია დოკუმენტის ფორმატების (ODF) ოჯახის რამდენიმე ქვეტიპიდან. ფორმატი მითითებულია, როგორც OASIS-ის მიერ გამოქვეყნებული და შენახული ODF 1.2 სპეციფიკაციების ნაწილი. Windows-ის და სხვა ოპერაციული სისტემების რიგ აპლიკაციებს შეუძლიათ ODS ფაილების გახსნა რედაქტირებისთვის და მანიპულირებისთვის, მათ შორის Microsoft Excel, NeoOffice და LibreOffice. ODS ფაილები ასევე შეიძლება გარდაიქმნას ცხრილების სხვა ფორმატებში, ისევე როგორც XLS, XLSX და სხვა სხვადასხვა აპლიკაციებით.

          link: "https://docs.fileformat.com/image/ods/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "მუშაობა სხვა პოპულარულ დოკუმენტის ფორმატებთან"
    content: |
        განაახლეთ ანოტაციის თვისებები ზოგიერთი პოპულარული ფაილის ფორმატიდან, როგორც ეს მოცემულია ქვემოთ.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/net/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/net/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/net/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/net/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/net/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/net/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/net/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/net/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/net/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/net/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/net/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/net/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/net/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/net/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/net/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/net/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/net/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/net/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/net/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/net/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/net/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/net/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/net/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/net/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/net/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/net/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/net/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/net/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/net/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/net/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/net/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/net/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/net/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/net/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/net/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---