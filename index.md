<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.6.3/css/all.css"
        integrity="sha384-UHRtZLI+pbxtHCWp1t77Bi1L4ZtiqrqD80Kn4Z8NTSRyMA2Fd33n5dQ8lWUE00s/" crossorigin="anonymous" />
    <title>My Presentation</title>
</head>

<body>

    <!-- Page 1 (Intro) -->
    <section id="page-1" class="page">
        <h1>Welcome To My Presentation</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Enim porro accusantium eligendi, ducimus voluptatum
            velit voluptatem accusamus facere sint facilis laudantium odit placeat, repellat commodi eius inventore
            delectus magni illo ex, nisi cumque corrupti consequatur architecto? Reiciendis officiis voluptatem illo.
        </p>
        <div>
            <a href="#page-2" class="btn">Next Page <i class="fas fa-arrow-circle-down"></i></a>
        </div>
    </section>

    <!-- Page 2 -->
    <section id="page-2" class="page">
        <h1>Page 2</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Enim porro accusantium eligendi, ducimus voluptatum
            velit voluptatem accusamus facere sint facilis laudantium odit placeat, repellat commodi eius inventore
            delectus magni illo ex, nisi cumque corrupti consequatur architecto? Reiciendis officiis voluptatem illo.
        </p>
        <div>
            <a href="#page-1" class="btn btn-dark">Prev Page <i class="fas fa-arrow-circle-up"></i></a>
            <a href="#page-3" class="btn">Next Page <i class="fas fa-arrow-circle-down"></i></a>
        </div>
    </section>

    <!-- Page 3 -->
    <section id="page-3" class="page">
        <h1>Page 3</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Enim porro accusantium eligendi, ducimus voluptatum
            velit voluptatem accusamus facere sint facilis laudantium odit placeat, repellat commodi eius inventore
            delectus magni illo ex, nisi cumque corrupti consequatur architecto? Reiciendis officiis voluptatem illo.
        </p>
        <div>
            <a href="#page-2" class="btn btn-dark">Prev Page <i class="fas fa-arrow-circle-up"></i></a>
            <a href="#page-4" class="btn">Next Page <i class="fas fa-arrow-circle-down"></i></a>
        </div>
    </section>

    <!-- Page 4 -->
    <section id="page-4" class="page">
        <h1>Page 4</h1>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Enim porro accusantium eligendi, ducimus voluptatum
            velit voluptatem accusamus facere sint facilis laudantium odit placeat, repellat commodi eius inventore
            delectus magni illo ex, nisi cumque corrupti consequatur architecto? Reiciendis officiis voluptatem illo.
        </p>
        <div>
            <a href="#page-3" class="btn btn-dark">Prev Page <i class="fas fa-arrow-circle-up"></i></a>

        </div>
    </section>

    <script src="https://code.jquery.com/jquery-3.4.1.min.js"
        integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"></script>

    <script>
        // Smooth Scrolling
        $('.btn').on('click', function (event) {
            if (this.hash !== '') {
                event.preventDefault();
                const hash = this.hash;
                $('html, body').animate({
                        scrollTop: $(hash).offset().top
                    },
                    800
                );
            }
        });
    </script>

</body>

</html>
