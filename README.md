# Learning

Here I list the books I plan to read and some ideas for personal projects.

## Books

### Coding

Steve McConnell
    *Code Complete (second edition)*.

Andrew Hunt, David Thomas
    *The pragmatic programmer*.

Glenfold J. Myers
    *The Art of Software Testing*.

Robert C. Martin
    *Agile Software Development, Principles, Patterns, and Practices*.

Felienne Hermans
    *The Programmer's Brain*.

### Programming languages

Scott Meyers
    *Effective STL: 50 Specific Ways to Improve Your Use of the Standard Template Library*.

Scott Meyers
    *Effective Modern C++: 42 Specific Ways to Improve Your Use of C++11 and C++14*.

### Software architecture

Eric Evans
    *Domain-Driven Design: Tackling Complexity in the Heart of Software*.

Humberto Cervantes
    *Designing Software Architectures: A Practical Approach*.

Len Bass, Rick Kazman, Paul Clemens
    *Software Architecture in Practice*.

Gregor Hohpe and Bobby Woolf
    *Enterprise Integration Patterns*.

.NET application architecture documentation
    https://docs.microsoft.com/en-us/dotnet/architecture/

Thomas Erl
    *Service-Oriented Architecture, Second Edition*.

Paul Clemens, Felix Bachmann, Len Bass, David Garlan, James Ivers, ..
    *Documenting Software Architectures: Views and Beyond*.

Sam Newmann
    *Building microservices*.

Martin Fowler
    *Patterns of Enterprise Application Architecture*.

### Computer science

Harold Abelson, Gerald Jay Sussman
    *Structure and Interpretation of Computer Programs*.

Open Web Application Security Project (OWASP)
    https://www.owasp.org

Aho, Alfred Vaino; Lam, Monica Sin-Ling; Sethi, Ravi; Ullman, Jeffrey David
    *Compilers: Principles, Techniques, and Tools (2 ed.)*.

### Processes and management

Matthew Skelton
    *Team Topologies*.

Fred Brooks
    *The Mythical Man-Month: Essays on Software Engineering*.

## Project ideas

### Photo manager

I have a lot of photos lying on a data storage in my home network.
They are accessible via smb. Since they are quite big, browsing through them
takes a long time and I struggle finding the photos, I am interested in.

This project consist of three parts. It is a web application which also uses
machine learning for picture classification.

The first part is a web application
which allows to browse to the folder structure of my photo storage.
The backend should resize the pictures to a smaller format and cache them
on the server side. It should provide endpoints for downloading
thumbnails and pictures in reduced size or in the original format.
The backend will resize and cache all the picture in one folder, as soon
one photo from that folder is requested. It should use an LRU caching strategy.

The second part will classify the photos with some tags (multiple labels
are possible), so that I can find things more quickly, without having to
browse through the folders. The web frondend needs to be able to assing
labels to the pictures. This should also be possible in batch (e.g. all the
picture in one folder get the same label). The labels needs to be persisted
on the backend. Finally it should be possible to search for all the pictures
with a given label. After a search, the server should only cache the search
results.

The third part is using machine learning to automatically classify new photos.
An model will be trained with the labels manually entered
by the user. When new pictures are added to the storage, the application
will automatically assign labels to the new files. The user should be able
to remove or add some labels (also in batch) and retrain the model.

#### Status

Not started yet.

### Personal page and CV

### Tides prediction

### Non violent communication

### Marathon passing times