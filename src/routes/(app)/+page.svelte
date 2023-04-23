<script>
    import Breadcrumbs from "$lib/components/Breadcrumbs.svelte";
    import Card from "$lib/components/Card.svelte";
    import Image from '$lib/components/Image.svelte'

    let items = [
        {
            name: "Home",
            href: "/"
        },
        {
            name: "News"
        }
    ]

    let haberler = [
        {
            id: "0",
            title: "Lorem Ipsum",
            desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Viverra accumsan in nisl nisi.",
            img: "https://picsum.photos/300/300?random=1",
            tipler: ["Minecraft", "Server"],
        },
        {
            id: "1",
            title: "Lorem Ipsum",
            desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Viverra accumsan in nisl nisi.",
            img: "https://picsum.photos/300/300?random=2",
            tipler: ["Minecraft", "Server"],
        },
        {
            id: "2",
            title: "Lorem Ipsum",
            desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Viverra accumsan in nisl nisi.",
            img: "https://picsum.photos/300/300?random=3",
            tipler: ["Minecraft", "Server"],
        }
    ]
</script>

<div class="p-4">
    <Breadcrumbs {items} />
    <div class="flex flex-col w-full lg:flex-row">
        <div class="grid flex-grow card rounded-box place-items-center">
            <div class="flex flex-row flex-wrap justify-center my-2 gap-8">
                <Card {haberler} />
            </div>
        </div> 
        <div class="divider lg:divider-horizontal"></div> 
        <div class="grid flex-grow card rounded-box lg:w-1/3">
            <div class="overflow-x-auto">
                <div class="btn ">Top Credit Purchasers</div>
                <table class="table table-zebra w-full my-2">
                  <!-- head -->
                  <thead>
                    <tr>
                      <th></th>
                      <th>Name</th>
                      <th class="text-center">Credit</th>
                    </tr>
                  </thead>
                  <tbody>
                    <!-- row 1 -->
                    <tr>
                      <th>1</th>
                      <td class="flex flex-wrap items-center gap-1">
                        <div class="avatar">
                          <div class="mask mask-squircle h-6 w-6">
                            <Image height="25" width="25" src="https://minotar.net/avatar/Efesso/25" title="Efesso"/>
                          </div>
                        </div>
                        Efesso
                      </td>
                      <td class="text-center">30</td>
                    </tr>
                    <!-- row 2 -->
                    <tr>
                      <th>2</th>
                      <td class="flex flex-wrap items-center gap-1">
                        <div class="avatar">
                          <div class="mask mask-squircle h-6 w-6">
                            <Image height="25" width="25" src="https://minotar.net/avatar/arian99/25" title="arian99"/>
                          </div>
                        </div>
                        arian99
                      </td>
                      <td class="text-center">20</td>
                    </tr>
                    <!-- row 3 -->
                    <tr>
                      <th>3</th>
                      <td class="flex flex-wrap items-center gap-1">
                        <div class="avatar">
                          <div class="mask mask-squircle h-6 w-6">
                            <Image height="25" width="25" src="https://minotar.net/avatar/LordTenebris/25" title="LordTenebris"/>
                          </div>
                        </div>
                        LordTenebris
                      </td>
                      <td class="text-center">10</td>
                    </tr>
                  </tbody>
                </table>
                <div class="divider"></div> 
                <div class="btn ">Last Credit Purchasers</div>
                <table class="table table-zebra w-full my-2">
                    <!-- head -->
                    <thead>
                      <tr>
                        <th></th>
                        <th>Name</th>
                        <th class="text-center">Credit</th>
                      </tr>
                    </thead>
                    <tbody>
                      <!-- row 1 -->
                      <tr>
                        <th>1</th>
                        <td class="flex flex-wrap items-center gap-1">
                          <div class="avatar">
                            <div class="mask mask-squircle h-6 w-6">
                              <Image height="25" width="25" src="https://minotar.net/avatar/Efesso/25" title="Efesso"/>
                            </div>
                          </div>
                          Efesso
                        </td>
                        <td class="text-center">30</td>
                      </tr>
                      <!-- row 2 -->
                      <tr>
                        <th>2</th>
                        <td class="flex flex-wrap items-center gap-1">
                          <div class="avatar">
                            <div class="mask mask-squircle h-6 w-6">
                              <Image height="25" width="25" src="https://minotar.net/avatar/arian99/25" title="arian99"/>
                            </div>
                          </div>
                          arian99
                        </td>
                        <td class="text-center">20</td>
                      </tr>
                      <!-- row 3 -->
                      <tr>
                        <th>3</th>
                        <td class="flex flex-wrap items-center gap-1">
                          <div class="avatar">
                            <div class="mask mask-squircle h-6 w-6">
                              <Image height="25" width="25" src="https://minotar.net/avatar/LordTenebris/25" title="LordTenebris"/>
                            </div>
                          </div>
                          LordTenebris
                        </td>
                        <td class="text-center">10</td>
                      </tr>
                    </tbody>
                  </table>
              </div>
        </div>
      </div>
</div>